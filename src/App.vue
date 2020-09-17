<template lang="pug">
  v-app
    Home
      router-view
</template>

<script>
import Home from '@/views/Home'

export default {
  name: 'App',

  components: {
    Home,
  },

  data: () => ({
    //
  }),
};
</script>