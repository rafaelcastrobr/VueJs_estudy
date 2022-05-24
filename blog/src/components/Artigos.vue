<template>
  <div class="hello">
    <div class="card" >
      <div class="post" v-for="artigo in artigos" v-bind:key="artigo.id">
        <h3>{{artigo.titulo}}</h3>
        <p>{{ artigo.conteudo }}</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "MeusArtigos",
  data() {
    return {
      artigos: [
        {
          id: 1,
          titulo: "Primeiro título",
          conteudo: "Conteúdo desse artigo 1",
        },
        {
          id: 2,
          titulo: "Segundo título",
          conteudo: "Conteúdo desse artigo 2",
        },
        {
          id: 3,
          titulo: "Terceiro título",
          conteudo: "Conteúdo desse artigo 3",
        },
      ],
    };
  },
  methods: {
    
  },

  created() {
   
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.hello {
  color: #333;
  padding: 20px;
  max-width: 1200px;
  margin: auto;
}

.card {
  background-color: #fff;
  color: #333;
}

.post {
  border: 1px solid silver;
  padding: 10px;
  margin-top: 10px;
  text-align: left;
}
</style>
