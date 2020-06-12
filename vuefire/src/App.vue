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
            <tr v-for="book in books" :key="book.id">
              <td>{{book.name}}</td>
              <td>{{subject}}</td>
            </tr>            
          </tbody>
        </table>
      </div>
    </div>
  </div>
</template>

<script>

import firebase from 'firebase'
import 'firebase/firestore'

let config = {
  apiKey: "AIzaSyA_CxHgD2-2xuetvevpq1-O7WiX2rEEBiY",
    authDomain: "books-aec36.firebaseapp.com",
    databaseURL: "https://books-aec36.firebaseio.com",
    projectId: "books-aec36",
    storageBucket: "books-aec36.appspot.com",
    messagingSenderId: "611515568318",
    appId: "1:611515568318:web:46159e93c9f479df620eef",
    measurementId: "G-RF1C6SKZR4"
}

// let app = Firebase.initializeApp(config);
// let db = app.database();

export const db = firebase
  // .initializeApp({ projectId : 'books-aec36'})
  .initializeApp(config)
  .firestore()


let bookRef = db.ref("books")

export default {
  name: "App",
  firebase : {
    books : bookRef
  },
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
