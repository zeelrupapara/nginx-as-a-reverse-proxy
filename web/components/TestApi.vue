<template>
  <div style="text-align: center; margin-top: 20rem">
    <h1> {{ api }} </h1>
  </div>
</template>

<script>
export default {
  data() {
    return {
      res: null,
    };
  },
  computed: {
    api() {
      return this.res;
    },
  },
  async created() {
    await this.$axios
      .get("http://localhost:8000/")
      .then((res) => {
        this.res = res.data;
      })
      .catch((err) => {
        this.res = err;
      });
  },
};
</script>
