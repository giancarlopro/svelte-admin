<script>
  import { Button, Col, Form, FormGroup, Input, Label, Row } from 'sveltestrap';
</script>

<Form>
  <FormGroup>
    <Label for="file">Arquivo:</Label>
    <Input type="file" name="file" id="file" />
  </FormGroup>

  <FormGroup>
    <Label for="profile">Perfil de Importação:</Label>
    <select id="profile" class="form-control">
      <option value="">Selecione</option>
      <option value="1">Aluno</option>
      <option value="2">Professor</option>
    </select>
  </FormGroup>

  <Button color="success">Importar</Button>
</Form>
