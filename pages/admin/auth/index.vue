<template>
<div class="ui container">
  <h1>Authentication</h1>
  <div class="ui yellow padded segment">
    <form class="ui form">
      <div class="field">
        <label>Email</label>
        <input type="email" name="email" placeholder="Email">
      </div>
      <div class="field">
        <label>Password</label>
        <input type="password" name="password" placeholder="Password">
      </div>
      <button class="ui primary button" type="submit">{{isLogin ? 'Login' : 'Sign Up'}}</button>
      <div @click="isLogin = !isLogin" class="ui animated yellow button" tabindex="0">
        <div class="visible content">Switch to {{isLogin ? 'Sign Up':'Login'}}</div>
        <div class="hidden content">
          <i class="right arrow icon"></i>
        </div>
      </div>
    </form>
  </div>
</div>
</template>

<script>
export default {
  name: 'AdminAuthPage',
  data() {
    return {
      isLogin: true
    }
  }
}
</script>

<style scoped>
.container {
  padding: 5%;
  text-align: center;
}

.ui.segment {
  max-width: 50%;
  margin-left: auto;
  margin-right: auto;
}
</style>
