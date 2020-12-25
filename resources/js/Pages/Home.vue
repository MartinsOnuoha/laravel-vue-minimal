<template>
  <div class="home">
    <img class="logo" width="100" src="logo.png" alt="">
    <h1>
      {{ count }}
    </h1>
    <button class="btn" @click="$store.commit('INCREMENT')">INCREMENT</button>
  </div>
</template>

<script>
import { mapState } from 'vuex';

export default {
  name: 'home',
  computed: {
    ...mapState({
      count: state => state.count
    }),
  }
}
</script>
