<template>
  <div class="category">
    {{ name }}
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
