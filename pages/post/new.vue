<template>
  <div>
    <PostForm :isNewPost=true />
  </div>
</template>

<script>
import PostForm from '../../components/forms/PostForm';

export default {
  components: {
    PostForm,
  },
}
</script>

<style lang="scss" src="./Post.scss">
