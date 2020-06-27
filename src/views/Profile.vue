<template>
  <div class="profile">
    <div class="profile-top">
      <img :src="images.myPhoto" class="myPhoto">
      <h2>
        Kaori Kohama<br>
        I am a software developer.
      </h2>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Profile',
  data(){
    return {
      images: {
        myPhoto: require("../assets/profile-image2.png")
      }
    }
  },
  components: {
    
  }
}
</script>

<style>

  .profile{
    text-align: center;
    align-items: center;
  }
  .profile-top{
    display: flex;
  }

  .myPhoto{
    height: 150px;
    width: 150px;
  }
</style>