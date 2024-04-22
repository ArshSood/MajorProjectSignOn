<template>
  <div class="signin-container">
    <h1>Welcome to my Application</h1>
    <button @click="showOptions" class="signin-btn">Sign In</button>
  </div>
</template>

<script>
export default {
  methods: {
    showOptions() {
      this.$emit('show-options', true);
    }
  }
}
</script>

<style>
.signin-container {
  max-width: 300px;
  margin: 0 auto;
}

h1 {
  text-align: center;
  margin-bottom: 20px;
}

.signin-btn {
  display: block;
  width: 100%;
  padding: 10px;
  background-color: #007bff;
  color: #fff;
  border: none;
  border-radius: 5px;
  cursor: pointer;
  font-size: 16px;
}

.signin-btn:hover {
  background-color: #0056b3;
}
</style>
