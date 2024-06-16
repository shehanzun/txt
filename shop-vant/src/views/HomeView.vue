<template>
  <div class="home">
    <img v-for="item in 10" alt="Vue logo" src="../assets/logo.png">
    <button @click="gotop">top</button>
  </div>
</template>

<style>
img {
  display: block;
  width: 200px;
  height: 300px;
  filter: drop-shadow(0px 0px 5px yellow);
}

button {
  background-color: blue;
  padding: 20px 30px;
  border-radius: 15px;
  color: white;
  border: none;
}
</style>

<script>
 export default{
  el: 'home',
  data() {
    return {
      val:false
    }
  },

  methods: {
    gotop() {
      this.val=true
      if (this.val) {
        
        window.scrollTo({
          top:899,
          behavior:'smooth'
        })
        this.val=false
      }
    },
  },
}

</script>
