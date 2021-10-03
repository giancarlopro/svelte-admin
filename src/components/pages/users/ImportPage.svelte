<script>
  import ImportForm from '../../organisms/users/ImportForm.svelte';
  import { Card, CardBody, CardHeader, Col, Row } from 'sveltestrap';
</script>

<Row>
  <Col md={12}>
    <Card class="mb-4">
      <CardHeader>
        <h6>Importar</h6>
      </CardHeader>

      <CardBody class="pt-0">
        <ImportForm />
      </CardBody>
    </Card>
  </Col>
</Row>
