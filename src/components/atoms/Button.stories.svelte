<script>
import { Meta, Story, Template } from '@storybook/addon-svelte-csf';
import Button from './Button.svelte';
</script>

<Meta
  title="Button"
  component={Button}
  argTypes={{
    label: { control: "text" },
    skin: {
      control: {
        type: "select",
        options: ["default", "primary", "secondary", "success", "danger", "warning", "info"]
      },
    },
    onClick: { action: "onClick" },
  }}
/>

<Template let:args>
  <Button {...args} on:click={args.onClick} />
</Template>

<Story
  name="Default"
  args={{
    skin: "default",
    label: "Button",
  }}
/>
