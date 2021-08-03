<template>
  <div>
    <NavBar />
    <main>
      <div class="container">
        <nuxt v-bind:time="time"/>
      </div>
    </main>


  </div>
</template>
<script>
import NavBar from '@@/components/NavBar.vue';
import timer from '@@/pages/timer.vue';
export default {
  data(){
    return{
      time:0,
    }
  },
  components:{
    NavBar,
    timer,
  },
  mounted:function(){
    this.$nextTick(function () {
    setInterval(()=>{
      this.time++;
    }, 1000)
  })
  }
}
</script>
