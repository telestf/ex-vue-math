<template>
  <div class="primo">
    <b-card bg-variant="primary">
      <h1>É primo?</h1>
      <h2>{{ calcula_primo(numero) }}</h2>
    </b-card>
  </div>
</template>

<script>
export default {
  name: 'Primo',
  props: {
    numero: Number
  },
  methods: {
    calcula_primo(n){
      let i = 0;
      for(i=2; i<n; i++){
        if(this.n%i === 0){
          return "Não"
        }
      }
      return "Sim"
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
