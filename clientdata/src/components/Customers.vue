<template>
  <div class="customers container">
    <h1 class="page-header">Gestionnaire de clientèle</h1>
    <table class="table table-striped">
      <thead>
        <tr>
          <th>Prénom</th>
          <th>Nom</th>
          <th>Email</th>
          <th></th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td>Anna</td>
          <td>Michelle</td>
          <td>am@gmail.com</td>
          <td></td>
        </tr>
      </tbody>
    </table>
  </div>
</template>

<script>
export default {
  name: "customers",
  data() {
    return {
      customers: [],
    };
  },
  methods: {
    fetchCustomers() {
      this.$http.get("http://slimapp/api/customers").then(function (response) {
        this.customers = JSON.parse(response.body);
      });
    },
  },
  created: function () {
    this.fetchCustomers();
  },
};
</script>

<style scoped></style>
