<template>
  <div>
    <PostForm :isNewPost=true />
  </div>
</template>

<script>
import Breadcrumbs from '../../components/Breadcrumbs';
import PostForm from '../../components/forms/PostForm';

export default {
  components: {
    Breadcrumbs,
    PostForm,
  },
}
</script>

<style lang="scss" src="./Post.scss">
