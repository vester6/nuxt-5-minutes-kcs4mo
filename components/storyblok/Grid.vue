<template>
  <div
    v-editable="blok"
    class="container mx-auto grid grid-cols-3 gap-6 place-items-center py-16"
  >
    <StoryblokComponent
      v-for="blok in blok.columns"
      :key="blok._uid"
      :blok="blok"
    />
  </div>
</template>

<script>
export default {
  props: ['blok'],
};
</script>
