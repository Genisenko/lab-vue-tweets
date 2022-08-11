<template>
  <div class="profile-image">
    <img
      :src="image"
      className="profile"
      alt="profile"
    />
   
  </div>
</template>

<script>

export default {
    props: {
      image:{
        type: String
      }
    }
  }
</script>

<style>

</style>