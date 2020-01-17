<template>
  <div class="home">
    <HelloWorld msg="Hello, Lisa"/>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/LastArticleComponent.vue';

export default {
  name: 'home',
  components: {
    HelloWorld,
  },
};
</script>
