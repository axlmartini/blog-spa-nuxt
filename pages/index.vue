<template>
  <div>
    <Slider />
    <PostsList />
  </div>
</template>

<script>
import Slider from '../components/Slider';
import PostsList from '../components/PostsList';
import {mapMutations} from 'vuex';

export default {
  components: {
    Slider,
    PostsList,
  },
  methods: {
    ...mapMutations('posts', ['setPosts']),
  },
  beforeRouteLeave: function(to, from, next) {
    this.setPosts([]);
    next();
  },
  middleware: ['postsList'],
}
</script>

