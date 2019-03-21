<template>
<div class="ui attached stackable menu">
  <div class="ui inverted secondary pointing menu">
    <nuxt-link to="/" class="item">
      Home
    </nuxt-link>
    <nuxt-link to="/posts" class="item">
      Blog
    </nuxt-link>
    <nuxt-link to="/about" class="item">
      About
    </nuxt-link>
    <nuxt-link to="/admin" class="item">
      Admin
    </nuxt-link>
  </div>
</div>
</template>

<style scoped>
.menu {
  background-color: rgb(11, 11, 11);
  padding: 10px;
}

.menu a.nuxt-link-exact-active {
  border-color: rgb(254, 240, 60) !important;
}
</style>
