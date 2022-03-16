<template>
  <div className="tweet">
    <ProfileImage :urlImage="tweet.user.image" />

    <div className="body">
      <div className="top">
        <User :userName="tweet.user.name" :userHandle="tweet.user.handle" />
        <Timestamp :timestamp="tweet.timestamp" />
      </div>
      <Message :message="tweet.message" />
      <Actions/>
    </div>
    <i class="fas fa-ellipsis-h"></i>
  </div>
</template>

<script>
import ProfileImage from "./ProfileImage.vue";
import Actions from "./Actions.vue";
import Message from "./Message.vue";
import Timestamp from "./Timestamp.vue";
import User from "./User.vue";
export default {
  components:{
    ProfileImage,
    Actions,
    Message,
    Timestamp,
    User
  },
  props:{
    tweet:{
      type: Object
    },
  },
  mounted(){
    console.log(this.tweet)
  }
}
</script>
<style scoped>
a {
  color: #42b983;
}
</style>
