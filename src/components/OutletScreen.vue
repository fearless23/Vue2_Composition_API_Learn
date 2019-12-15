<template>
  <div class="outletScreen">
    <div class="header">
      <!-- <div class="userIcon">
                <img src="../images/user.png" class="userImg">
      </div>-->
      <div class="customerInfo">
        <div class="row userMessage">hello {{userName}}</div>
        <div class="row customerMessage">welcom to {{customerName}}</div>
      </div>
    </div>
    <div class="outletsContainer">
      <div v-for="k in outlets" class="outlet" v-bind:key="k.outletID">{{k.outletID}}</div>
    </div>
    <div class="logout">logout</div>
  </div>
</template>


<script lang="ts">
import { Component, Prop, Vue } from "vue-property-decorator";

@Component
export default class OutletScreenTmpl extends Vue {
  @Prop() private userName!: string;
  @Prop() private customerName!: string;
  @Prop() private outlets!: { name: string; outletID: string };
}
</script>


<style scoped>
</style>
