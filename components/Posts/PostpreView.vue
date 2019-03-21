<template>
<div class="ui card">
  <div class="image">
    <img :src="thumbnail" :alt="title">
  </div>
  <div class="content">
    <nuxt-link :to="postLink" class="header">{{title}}</nuxt-link>
    <div class="description">
      {{previewText}}
    </div>
  </div>
</div>
</template>

<script>
export default {
  name: 'PostPreview',
  props: {
    id: {
      type: String,
      required: true
    },
    isAdmin: {
      type: Boolean,
      required: true
    },
    title: {
      type: String,
      required: true
    },
    previewText: {
      type: String,
      required: true
    },
    thumbnail: {
      type: String,
      required: true
    }
  },
  computed: {
    postLink() {
      return this.isAdmin ? '/admin/' + this.id : '/posts/' + this.id
    }
  }
}
</script>
