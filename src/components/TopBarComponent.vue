<template>
    <div>
        <vs-navbar collaspe v-model="activeItem" class="navbarx" type="border">
            <div slot="title">
                <vs-button @click="toggleSidebar(true)"
                    color="dark" type="flat" radius icon="menu" />
                <vs-spacer></vs-spacer>
                <vs-navbar-title class="navbarx-title">
                    <h2>HOOMEGA LOGO</h2>
                </vs-navbar-title>
            </div>
            <vs-navbar-item class="navbarx-item" index="0">
                <a href="#">SEARCH</a>
                <span class="vs-navbar-after"></span>
            </vs-navbar-item>
            <vs-navbar-item class="navbarx-item" index="1">
                <a href="#">CATEGORIES</a>
                <span class="vs-navbar-after"></span>
            </vs-navbar-item>
            <vs-navbar-item class="navbarx-item" index="2">
                <a href="#">ARCHIVES</a>
                <span class="vs-navbar-after"></span>
            </vs-navbar-item>
        </vs-navbar>
        <vs-sidebar parent="body"
            default-index="1" color="primary" class="sidebarx" spacer v-model="toggle">
            <div class="blank-space" />
            <vs-divider/>
        </vs-sidebar>
    </div>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator';
@Component
export default class TopBarComponent extends Vue {
    private activeItem: number = 0;

    private toggle: boolean = false;

    private toggleSidebar(toggle: boolean) {
      this.toggle = toggle;
    }
}
</script>

<style lang="less">
@media screen and (min-width: 800px) {
    .navbarx {
        letter-spacing: .3rem;
        height: 100px;
        padding: 0 50px;
        font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Cantarell, 'Open Sans';
        font-weight: 400;

        .navbarx-title {
            display: flex;
            justify-content: space-between;
        }

        .blank-space {
            height: 100px;
        }
    }
}
</style>
