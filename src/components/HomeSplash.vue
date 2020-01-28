<!-- @format -->

<template>
  <vs-row vs-w="11">
    <vs-col vs-offset="1">
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
              <p class="textbox-description">
                What if you sailed between serenity and efficiency through a unique, personalized
                organization: yours?
              </p>
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
    </vs-col>
  </vs-row>
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
  background: url(https://images.pexels.com/photos/373076/pexels-photo-373076.jpeg) no-repeat center
    center;
  background-size: cover;
  border: 0;
  border-radius: 15px;
  width: 100%;
  height: 80vh;

  .homepage-textbox {
    position: relative;
    top: 50%;

    .textbox-copyright {
      font-size: calc(10px + (26 - 14) * ((100vw - 300px) / (1600 - 300)));
      line-height: calc(1.3em + (1.5 - 1.2) * ((100vw - 300px) / (1600 - 300)));
      font-weight: 100;
    }
    .textbox-headline {
      font-size: calc(32px + (26 - 14) * ((100vw - 300px) / (1600 - 300)));
      line-height: calc(1.3em + (1.5 - 1.2) * ((100vw - 300px) / (1600 - 300)));
      font-weight: 500;
    }
    .textbox-description {
      font-size: calc(8px + (26 - 14) * ((100vw - 300px) / (1600 - 300)));
      line-height: calc(1.3em + (1.5 - 1.2) * ((100vw - 300px) / (1600 - 300)));
      font-weight: 200;
    }
  }
}
</style>
