<template>
  <div id="card">
    <div class="centering">
      <Mycards v-for="album,i in listaalbum"
      :key="i"
      :details="album"/>
      
    </div>
  </div>
</template>

<script>
import axios from "axios";
import Mycards from "@/components/Mycards.vue";
export default {
  name: "Mycontainer",
  components: {
    Mycards,
  },
  data() {
    return {
      apiUrl: "https://flynn.boolean.careers/exercises/api/array/music",
      listaalbum: [],
    };
  },
  created() {
    this.getinfo();
  },
  methods: {
    getinfo() {
      axios
      .get(this.apiUrl)
      .then((result) => {
        this.listaalbum = result.data.response
      });
    },
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
#card {
  background-color: rgb(32, 49, 65);
  height: auto;
}
.centering {
  width: 70%;
  margin: 0 auto;
  display: flex;
  flex-wrap: wrap;
}
</style>