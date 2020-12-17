<template>
  <div class="add container">
    <h1>Ajouter un client</h1>
    <form v-on:submit="addCustomer">
      <div class="well">
        <h4>Informations</h4>
        <div class="form-row">
          <div class="form-group col-md-6">
            <label>Prénom</label>
            <input type="text" class="form-control" placeholder="Prénom" />
          </div>
          <div class="form-group col-md-6">
            <label>Nom</label>
            <input type="text" class="form-control" placeholder="Nom" />
          </div>
        </div>
        <div class="form-row">
          <div class="form-group col-md-6">
            <label>Email</label>
            <input type="text" class="form-control" placeholder="Email" />
          </div>
          <div class="form-group col-md-6">
            <label>Téléphone</label>
            <input type="text" class="form-control" placeholder="Téléphone" />
          </div>
        </div>
      </div>
      <div class="well">
        <h4>Lieu</h4>
        <div class="form-group">
          <label>Adresse</label>
          <input type="text" class="form-control" placeholder="Adresse" />
        </div>
        <div class="form-group">
          <label>Ville</label>
          <input type="text" class="form-control" placeholder="Ville" />
        </div>
        <div class="form-group">
          <label>Code postal</label>
          <input type="text" class="form-control" placeholder="Code postal" />
        </div>
      </div>
      <button type="submit" class="btn btn-primary">Ajouter</button>
    </form>
  </div>
</template>

<script>
export default {
  name: "add",
  data() {
    return {};
  },
};
</script>

<style scoped></style>