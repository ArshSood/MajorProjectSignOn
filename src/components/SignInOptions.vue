<template>
  <div v-if="showOptions" class="options-container">
    <h1>Sign-In Options</h1>
    <button @click="signInWithGoogle" class="signin-option">Sign In with Google</button>
    <button @click="signInWithTimelessVisage" class="signin-option">Sign In with Timeless Visage</button>
  </div>
</template>

<script>
export default {
  data() {
    return {
      showOptions: true
    };
  },
  methods: {
    signInWithGoogle() {
      // Implement sign-in with Google logic
      console.log('Signing in with Google');
    },
    signInWithTimelessVisage() {
      // Implement sign-in with Timeless Visage logic
      console.log('Signing in with Timeless Visage');
    }
  }
}
</script>

<style>
.options-container {
  max-width: 300px;
  margin: 0 auto;
  text-align: center;
}

.signin-option {
  display: block;
  width: 100%;
  padding: 10px 20px;
  margin-top: 10px;
  background-color: #28a745;
  color: #fff;
  border: none;
  border-radius: 5px;
  cursor: pointer;
  font-size: 16px;
}

.signin-option:hover {
  background-color: #218838;
}
</style>
