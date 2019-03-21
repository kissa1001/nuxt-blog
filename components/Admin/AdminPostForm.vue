<template>
<div class="ui container">
  <div class="ui yellow piled segment">
    <form @submit.prevent="onSave" class="ui form">
      <div class="field">
        <label>Author Name</label>
        <input v-model="editedPost.author" type="text" name="author-name" placeholder="Author Name">
      </div>
      <div class="field">
        <label>Title</label>
        <input v-model="editedPost.title" type="text" name="title" placeholder="Title">
      </div>
      <div class="field">
        <label>Thumbnail Link</label>
        <input v-model="editedPost.thumbnailLink" type="text" name="title" placeholder="Thumbnail Link">
      </div>
      <div class="field">
        <label>Content</label>
        <textarea name="content" v-model="editedPost.content"></textarea>
      </div>
      <button class="ui primary button" type="submit">Submit</button>
      <button class="ui button" type="submit" @click="onCancel">Cancel</button>
    </form>
  </div>
</div>
</template>

<script>
export default {
  props: {
    post: {
      type: Object,
      required: false
    }
  },
  data() {
    return {
      editedPost: this.post ? {
        ...this.post
      } : {
        author: '',
        title: '',
        thumbnailLink: '',
        content: ''
      }
    }
  },
  methods: {
    onSave() {
      console.log(this.editedPost);
    },
    onCancel() {
      this.$router.push('/admin');
    }
  }
}
</script>

<style scoped>
.container {
  display: flex;
  justify-content: center;
  padding: 5%;
}

.segment {
  width: 100%;
}
</style>
