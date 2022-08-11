<template>
  <div className="tweet">

    <ProfileImage :image="user.image" />

    <div className="body">
      <div className="top">

        <User :user="user" />
        <Timestamp :timestamp="timestamp" />

      </div>

      <Message :message="message" />

      <Actions />
    </div>

    <i class="fas fa-ellipsis-h"></i>
  </div>
</template>

<script>
import User from './User.vue';
import Timestamp from './Timestamp.vue';
import ProfileImage from './ProfileImage.vue';
import Message from './Message.vue';
import Actions from './Actions.vue';




export default {
  name: "Tweet",
  components: {
    User,
    Timestamp,
    ProfileImage,
    Message,
    Actions
},
  props: {
    image: String,
    user: Object,
    timestamp: String,
    message: String,
  },
}
</script>

<style>
a {
  color: #42b983;
}
</style>
