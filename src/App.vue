<template>
  <div class="app container">
    <ul>
      <li>{{ number + 1 }}</li>
      <li>Value of ok var is: {{ ok ? 'true' : 'false' }}</li>
      <li>{{ message.split('').reverse().join('') }}</li>
    </ul>
    <span v-if="visible">Now you see me</span>
  </div>
</template>

<script>
  export default {
    name: "App",
    data: () => ({
      message: "Powered by MD!",
      number: 5,
      ok: true,
      visible: true,
    })
  };
</script>

<style>
  .app {
    margin: 0 auto;
    font-family: sans-serif;
    background-color: #ccf7e2;
    padding: 10px;
    border-radius: 5px;
    max-width: 500px;
  }
</style>
