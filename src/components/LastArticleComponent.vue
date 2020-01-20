<template>
  <div class="homepage-showcase">
    <div class="homepage-textbox">
      <vs-row vs-w="12">
        <vs-col vs-offset="1" vs-type="flex" vs-justify="left" vs-align="left" vs-w="4">
          <p class="textbox-copyright">2020 · All rights reserved.</p>
        </vs-col>
      </vs-row>
      <vs-row vs-w="12">
        <vs-col vs-offset="1" vs-type="flex" vs-justify="left" vs-align="left" vs-w="6">
          <p class="textbox-headline">ORGANIZATION 💙 PRODUCTIVITY.</p>
        </vs-col>
      </vs-row>
      <vs-row vs-w="12">
        <vs-col vs-offset="1" vs-w="4">
          <p class="textbox-description">What if you sailed between serenity and efficiency
through a unique, personalized organization: yours?</p>
        </vs-col>
      </vs-row>
      <br />
      <vs-row vs-w="12">
        <vs-col vs-offset="1" vs-w="4">
          <vs-button color="primary" type="filled" icon="mail">
            CONTACT ME
          </vs-button>
        </vs-col>
      </vs-row>
    </div>
  </div>
</template>

<script lang="ts">
import { Component, Prop, Vue } from 'vue-property-decorator';

@Component
export default class LastArticleComponent extends Vue {
  @Prop() private msg!: string;
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="less">
.homepage-showcase {
  background: url(https://images.pexels.com/photos/373076/pexels-photo-373076.jpeg) no-repeat center center;
  background-size: cover;
  width: 100%;
  height: 805px;

  .homepage-textbox {
    position: relative;
    top: 50%;

    .textbox-copyright {
      font-size: 15px;
      font-weight: 100;
    }
    .textbox-headline {
      font-size: 50px;
      font-weight: 500;
    }
    .textbox-description {
      font-size: 25px;
      font-weight: 200;
    }
  }
}
</style>
