<!-- @format -->

<template>
  <div class="home">
    <HomeSplash msg="Hello, Lisa" />
    <ArticlesList msg="Hello, Lisa" />
  </div>
</template>

<script>
// @ is an alias to /src
import HomeSplash from '@/components/HomeSplash.vue';
import ArticlesList from '@/components/ArticlesList.vue';

export default {
  name: 'home',
  components: {
    HomeSplash,
    ArticlesList,
  },
};
</script>
