<template>
  <div id="app">
   <app-message></app-message>
   <hr>
   <router-link to="/">Home</router-link>
   <router-link to="/users/10">Users for team 10</router-link>
   <router-link to="/users/12">Users for team 12</router-link>
   <hr>
   <router-view></router-view>
  </div>
</template>

<script>
export default {
  data () {
    return {
    }
  }
}
</script>

<style lang="scss">
</style>
