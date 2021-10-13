<template>
  <div>
    <CarCards :cars="cars" @reload="$emit('reload')"></CarCards>
  </div>
</template>

<script>
import CarCards from '@/components/CarCards.vue';

export default {
  name: 'Home',
  props: {
    cars: {
      type: Array,
    },
  },
  components: {
    CarCards,
  },
};
</script>
