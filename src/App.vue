<template>
  <div>
    <Navbar />
    <div v-from="task in atividades">
      <Card :tarefa="task"/>
    </div>
  </div>
</template>

<script>
import Navbar from "./components/Navbar.vue";
import atividades from "./assets/atividades.json";
import Card from "./components/Cardes.vue";
export default {
  name: "App",
  components: {
    Navbar,
    Card
  },
  data() {
    return {
      atividades
    };
  }
};
</script>
