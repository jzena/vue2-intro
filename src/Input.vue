<template>
  <div>
    <input type="text" :value="msg" @input="changeMessage" />
    <p>{{messageInput}}</p>
  </div>
</template>

<script>
export default {
  props: ["msg"],
  data() {
    return {
      messageInput: ""
    };
  },
  methods: {
    changeMessage(event) {
      this.messageInput = event.target.value;
      this.$emit('messageChanged', this.messageInput);
    }
  }
};
</script>