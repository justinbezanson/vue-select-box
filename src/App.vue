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
</template>

<style scoped>

</style>
