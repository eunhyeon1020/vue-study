<template>
  <div>
    <app-header 
    v-bind:propsdata="str"
    v-on:renew="renewStr">
    </app-header>
  </div>
</template>

<script>
import AppHeader from './components/AppHeader.vue';

export default {
  components: {
    'app-header' : AppHeader
  },

  data: () => ({
    str: '넘어온거니'
  }),
  methods: {
    renewStr: function() {
      this.str = 'hi'
    }
  }

  

} 
</script>

<style>

</style>