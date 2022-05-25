<template>
  <div class="about">
    <h1>Diga quem eu sou</h1>
    <input type="text" v-model="sobre">
    <input type="button" value="Salvar" v-on:click="save"/>
  </div>
</template>


<script>
export default {
  data () {
    return {
      sobre: ''
    }
  },
  mounted() {
    if(localStorage.about) {
      this.sobre = localStorage.getItem('about')
    } 
  },
  methods: {
    save () {
      localStorage.setItem('about', this.sobre)
    }
  }
}
</script>