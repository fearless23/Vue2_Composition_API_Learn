<template>
  <div class="loginPageContainer">
    <div class="logo">{{name}}</div>
    <div class="login" id="abc">
      <div class="form">
        <input type="text" class="inputRow userID" data-id="userID" placeholder="User ID" />
        <input
          type="password"
          onclick="scrollLogin()"
          class="inputRow password"
          data-id="password"
          placeholder="Password"
        />
      </div>
      <div class="loginBtn">Submit</div>
    </div>
  </div>
</template>

<script lang="ts">
import { Component, Prop, Vue } from "vue-property-decorator";

@Component
export default class LoginTmpl extends Vue {
  @Prop() private name!: string;
}
</script>


<style scoped>

</style>
