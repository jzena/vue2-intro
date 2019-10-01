<template>
  <div class="messageComponent">
    <h1>{{message}}</h1>
    <app-input :msg="message" @messageChanged="message = $event" />
  </div>
</template>
<script>
import Input from "./Input";
export default {
  data() {
    return {
      message: "Welcome to vuejs tutorial!"
    };
  },
  components: {
    "app-input": Input
  }
};
</script>
<style scoped>
.messageComponent {
  border: 1px solid whitesmoke;
  margin: 5px;
  padding: 5px;
}
</style>