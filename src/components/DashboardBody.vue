<template>
  <div class="innerContainer">
    <div class="header">
      <div class="home">
        <img src="@/assets/imgs/menu.png" class="homeIcon" />
      </div>
      <div class="customerName"></div>
      <div class="syncBtn">
        <img src="@/assets/imgs/sync.png" class="syncIcon" />
      </div>
    </div>
    <div class="contentContainer">
      <div class="infoContainer"></div>
    </div>
  </div>
</template>


<script lang="ts">
import { Component, Prop, Vue } from "vue-property-decorator";

@Component
export default class DashboardBodyTmpl extends Vue {
  @Prop() private userName!: string;
  @Prop() private customerName!: string;
  @Prop() private outlets!: { name: string; outletID: string };
}
</script>


<style scoped>
</style>
