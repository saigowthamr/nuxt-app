<template>
  <div>
    <h1>This is the About page</h1>
    <p>{{$route.query.name}}</p>
  </div>
</template>

<script>
export default {
  head() {
    return {
      title: "About page",
      htmlAttrs: {
        lang: "ar",
      },
    };
  },
  created() {
    console.log(this.$route.query.name);
  },
};
</script>