<template>
  <div id="app" class="container">
    <SignIn v-if="!showOptions" @show-options="handleShowOptions" />
    <SignInOptions v-else />
  </div>
</template>

<script>
import SignIn from './components/SignIn.vue';
import SignInOptions from './components/SignInOptions.vue';

export default {
  name: 'App',
  components: {
    SignIn,
    SignInOptions
  },
  data() {
    return {
      showOptions: false
    };
  },
  methods: {
    handleShowOptions(value) {
      this.showOptions = value;
    }
  }
}
</script>

<style>
.container {
  max-width: 600px;
  margin: 50px auto;
  padding: 20px;
  border: 1px solid #ccc;
  border-radius: 10px;
  background-color: #f8f9fa;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
}

h1 {
  text-align: center;
  margin-bottom: 20px;
}

button {
  display: inline-block;
  padding: 10px 20px;
  background-color: #007bff;
  color: #fff;
  border: none;
  border-radius: 5px;
  cursor: pointer;
  font-size: 16px;
}

button:hover {
  background-color: #0056b3;
}
</style>
