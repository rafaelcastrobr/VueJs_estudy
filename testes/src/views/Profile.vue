<template>
  <div class="home">
    <h1>Profile</h1>
    <h3>Rafael</h3>
    <span>
      {{ this.$route.params.username }}
    </span>
    <h1>{{ nome }}</h1>
  </div>
</template>

<script>
export default {
  name: "ProfileVue",
  data() {
    return {
      nome: "",
    };
  },
  mounted() {
    this.nome = localStorage.getItem("about");
  },
};
</script>