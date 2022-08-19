<template>
  <div>
    <div v-for="(data, index) in data" :key="index">
      {{ data[`data`][`first_name`] }}
    </div>
  </div>
</template>

<script>
import axios from "axios";
export default {
  mounted() {
    axios
      .request({
        url: `https://reqres.in/api/users`,
      })
      .then((response) => {
        response;
      })
      .catch((error) => {
        error;
      });
  },
};
</script>

<style scoped>
</style>