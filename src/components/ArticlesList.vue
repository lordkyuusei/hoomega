<!-- @format -->

<template>
  <div>
    <vs-row vs-w="12">
      <vs-col vs-offset="1" vs-justify="center" vs-align="center" vs-w="10"
        ><vs-divider
          ><vs-button color="primary" type="filled" icon="arrow_downward"></vs-button></vs-divider
      ></vs-col>
    </vs-row>
    <vs-row class="article-list" vs-w="11" type="flex" vs-align="center" vs-justify="center">
      <vs-col
        vs-offset="1"
        vs-w="4"
        type="flex"
        vs-align="center"
        vs-justify="center"
        :key="index"
        v-for="(card, index) in 9"
        vs-lg="3"
        vs-sm="5"
        vs-xs="12"
      >
        <ArticlePreview
          header="Title of the awesome article"
          content="short description of the article"
        />
      </vs-col>
    </vs-row>
  </div>
</template>

<script lang="ts">
import { Component, Vue, Prop } from 'vue-property-decorator';
import ArticlePreview from './ArticlePreview.vue';

@Component({
  components: {
    ArticlePreview,
  },
})
export default class ArticleList extends Vue {}
</script>

<style scoped lang="less">
.article-list {
}
</style>
