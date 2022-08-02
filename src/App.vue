<template>
  <div class="global-container">
    <Message initMessage="Hello world" />
  </div>
</template>

<script>
import Message from "@/components/Message.vue";
export default {
  name: 'App',
  components: {
    Message
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}

.global-container {
  padding: 2rem;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}
</style>
