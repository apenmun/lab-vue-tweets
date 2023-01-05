<template>
  <div className="tweet">
    <img src="{{image}}" className="profile" alt="profile" />

    <div className="body">
      <div className="top">
        <span className="user">
          <User :name="name" />
          <User :handle="handle" />
        </span>

        <span className="timestamp">{{ timestamp }}</span>
      </div>

      <p className="message">
        <Message :message="message" />
      </p>

      <div className="actions">
        <!-- Font Awesome icons -->
        <i class="far fa-comment"></i>
        <i class="fas fa-retweet"></i>
        <i class="far fa-heart"></i>
        <i class="fas fa-share"></i>
      </div>
    </div>

    <i class="fas fa-ellipsis-h"></i>
  </div>
</template>

<script setup>
import User from "./User.vue";
const props = defineProps(["name", "handle", "timestamp", "message", "image"]);
</script>

<style scoped>
a {
  color: #42b983;
}
</style>
