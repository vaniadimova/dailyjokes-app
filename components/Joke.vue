<template>
  <nuxt-link :to="'jokes/' + id">
    <div class="joke">
      <p>{{ joke }}</p>
    </div>
  </nuxt-link>
</template>

<script>
export default {
  name: "Joke",
  props: ["joke", "id"]
};
</script>

<style>
.joke {
  padding: 1rem;
  font-size: 1.4rem;
   color: #15083a;
  border: 1px dotted rgb(141, 137, 137);
  margin: 1rem 0;
}
</style>