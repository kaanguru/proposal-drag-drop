<template>
  <SlickList axis="y" v-model:list="fruits">
    <SlickItem v-for="(fruit, i) in fruits" :key="fruit" :index="i">
      {{ fruit }}
    </SlickItem>
  </SlickList>
</template>

<script lang="ts">
import { SlickList, SlickItem } from 'vue-slicksort';

export default {
  components: {
    SlickList,
    SlickItem,
  },
  data() {
    return {
      fruits: ['Apples', 'Bananas' /* etc. */],
    };
  },
};
</script>
