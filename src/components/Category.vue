<template>
  <div class="category">
      <h1>{{ name }}</h1>
      <p>Auto Cancellation allows you to only run builds for the latest commits in the queue. This setting can be applied to builds for Branch builds and Pull Request builds separately. Builds will only be canceled if they are waiting to run, allowing for any running jobs to finish.</p>
  </div>
</template>
<style>
.category {
  padding: 5px 10px;
}
.category p {
  background: #d16363;
  color: #dddddd;
  padding: 10px;
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
