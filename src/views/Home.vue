<template>
  <div class="home">
    <Nav />
    <Card />
    <Button
      :rounded="true"
      custom-class="bg-transparent hover:bg-blue-500 text-blue-700 font-semibold hover:text-white py-2 px-4 border border-blue-500 hover:border-transparent rounded"
    >
      a
    </Button>
  </div>
</template>

<script>
// @ is an alias to /src
import Nav from '@/components/Nav.vue';
import Card from '@/components/Card.vue';
import Button from '@/components/Button.vue';

export default {
  name: 'Home',
  components: {
    Nav,
    Card,
    Button,
  },
};
</script>
