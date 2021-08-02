<template>
  <div>
    <NavBar />
    <main>
      <div class="container">
        <nuxt />
      </div>
    </main>


  </div>
</template>
<script>
import NavBar from '@@/components/NavBar.vue';
export default {
  components:{
    NavBar,
  }
}
</script>
