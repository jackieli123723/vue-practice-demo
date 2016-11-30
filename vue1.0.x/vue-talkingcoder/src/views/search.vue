<template>
  <div>
     <header-tab icon="settings" title="发现">
       
    </header-tab>
    <div class="img-area">
      <img src="../../static/img/me/large.jpg">
    </div>
    <div class="hello">
      <h1>{{ msg }}</h1>
    </div>

  </div>
</template>

<script>
import HeaderTab from '../components/HeaderTab.vue';
export default {
  data () {
    return {
      // note: changing this line won't causes changes
      // with hot-reload because the reloaded component
      // preserves its current state and we are modifying
      // its initial state.
      msg: 'message!'
    }
  },
  components:{
    HeaderTab
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

  h1 {
    color: #42b983;
  }
  .img-area{
    width: 100%;

  }
  .img-area img{
    width: 100%;
    height:9rem;
    display: block;
  }

</style>
