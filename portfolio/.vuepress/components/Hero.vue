<template>
  <h1 v-if="text" class="title" v-html="text" />
</template>

<script>
export default {
  props: {
    text: {
      type: String,
      required: false
    }
  }
}
</script>

<style scoped>
  .title {
    text-align: center;
    font-size: calc(21px + (48 - 14) * ((100vw - 300px) / (1600 - 300)));
    font-weight: 300;
    line-height: 1.25;
    letter-spacing: 0.1rem;
    width: 800px;
    max-width: 100%;
    margin: 6rem auto 2rem auto;
  }

  @media screen and (min-width: 768px) {
    .title {
      margin: 12vw auto 7vw auto;
    }
  }

</style>
