<template>
  <div class="category">
      <h1>{{ name }}</h1>
    
  </div>
</template>
<style>
.category {
  width: 300px;
}
</style>
<script>
import { mapState } from 'vuex';

export default {
  computed: {
    ...mapState({
      name: state => state.name
    })
  }
}
</script>
