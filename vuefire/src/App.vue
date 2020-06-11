<template>
  <div id="app">
    <!-- <h2>working</h2> -->
    <div class="card">
      <div class="card-header">
        <h3>randevular</h3>
      </div>
      <div class="card-bod">
        <table class="table">
          <thead class="thead-dark">
            <tr>
              <th scope="col">isim</th>
              <th scope="col">konu</th>
              <th scope="col">işlem</th>
            </tr>
          </thead>
          <tbody>
            <tr>
              <td>Mark</td>
              <td>Otto</td>
              <td>@mdo</td>
            </tr>
            <tr>
              <td>Jacob</td>
              <td>Thornton</td>
              <td>@fat</td>
            </tr>
            <tr>
              <td>Larry</td>
              <td>the Bird</td>
              <td>@twitter</td>
            </tr>
          </tbody>
        </table>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "App",
  components: {},
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
