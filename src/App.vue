<script setup>
import { ref } from 'vue'
import SelectBox from './components/SelectBox.vue';

const countries = [
  {
    value: 'CA',
    label: 'Canada',
    avatar: '/flags/CA.svg'
  },
  {
    value: 'US',
    label: 'United States',
    avatar: '/flags/US.svg'
  }
];

const country = ref({})
</script>

<template>
  <div class="sm:max-w-md p-8">
    <SelectBox :options="countries" v-model="country" placeholder="Select Country" />
  </div>

  <div class="sm:max-w-md p-8 pt-0">
    Source: <a href="https://github.com/justinbezanson/vue-select-box" class="text-blue-600 underline underline-offset-1 hover:no-underline">Github</a>
  </div>
</template>

<style scoped>

</style>
