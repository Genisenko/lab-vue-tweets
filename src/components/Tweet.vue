<template>
  <div className="tweet">
    <ProfileImage :image="user.image"/>

    <div className="body">
      <div className="top">
        <User :user="user" />
        <Timestamp :time="time" />
      </div>

      <Message :message="message" />

      <Action  />
      
    </div>

    <i class="fas fa-ellipsis-h"></i>
  </div>
</template>

<script>
import ProfileImage from './ProfileImage.vue';
import User from './User.vue';
import Timestamp from './Timestamp.vue';
import Message from './Message.vue';
import Action from './Action.vue';
  export default {
    props: {
      message: String,
      timestamp: String,
      user: Object,
    },
    components: { ProfileImage, User, Timestamp, Message, Action }
}
</script>

<style scoped>
a {
  color: #42b983;
}
</style>
