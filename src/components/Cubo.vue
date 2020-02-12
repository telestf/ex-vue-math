<template>
  <div class="cubo">
    <b-card bg-variant="danger">
      <h1>Cubo</h1>
      <h2>{{ calcula_cubo(numero) }}</h2>
    </b-card>
  </div>
</template>

<script>
export default {
  props: {
    numero: Number
  },
  methods: {
    calcula_cubo(n){
      return n**3
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
