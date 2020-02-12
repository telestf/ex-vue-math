<template>
  <div class="Fatorial">
    <b-card bg-variant="secondary">
      <h1>Fatorial</h1>
      <h2>{{ calcula_fatorial(numero) }}</h2>
    </b-card>
  </div>
</template>

<script>
export default {
  name: 'Fatorial',
  props: {
    numero: Number
  },
  methods: {
    calcula_fatorial(n){
      let i = 0;
      let resultado = 1;
      for(i=1; i<n+1; i++){
        resultado *= i
      }
      return resultado
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
