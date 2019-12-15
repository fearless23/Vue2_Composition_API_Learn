<template>
  <div>
    <div class="mainContainer">
      <!-- <LoginTmpl name="QuickPOS" /> -->
      <OutletScreenTmpl :userName="userName" :customerName="customerName" :outlets="outlets" />
    </div>
  </div>
</template>

<script>
import LoginTmpl from "@/components/Login.vue";
import OutletScreenTmpl from "@/components/OutletScreen";

export default {
  name: "home",
  components: {
    LoginTmpl,
    OutletScreenTmpl,
  },
  data: () => {
    return {
      userName: "pind",
      customerName: "Pind",
      outlets: [{ name: "Pind", outletID: "BANGALORE" }]
    };
  }
};
</script>
