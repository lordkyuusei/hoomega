<!-- @format -->

<template>
  <vs-card actionable class="cardx" fixedHeight>
    <div slot="header">
      <h3>{{ header }}</h3>
    </div>
    <div slot="media">
      <img src="https://cataas.com/cat" />
    </div>
    <div>
      <span>{{ content }}</span>
    </div>
    <div slot="footer">
      <vs-row vs-justify="flex-end">
        <span>By <strong>@lisa.dps</strong> on <i> a certain date</i></span>
      </vs-row>
    </div>
  </vs-card>
</template>

<script lang="ts">
import { Component, Prop, Vue } from 'vue-property-decorator';

@Component({})
export default class ArticlePreview extends Vue {
  @Prop(String) private header!: string;

  @Prop(String) private content!: string;
}
</script>

<style lang="less"></style>
