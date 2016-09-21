<template>
  <main id="app" class="app-container">
    <h1>MARKS</h1>

    <data-decryptor></data-decryptor>
  </main>
</template>

<script type="text/ecmascript-6">
  import DataDecryptor from './components/DataDecryptor'

  export default {
    components: {
      DataDecryptor
    }
  }
</script>

<style lang="scss">
  html {
    height: 100%;
  }

  body {
    align-items: center;
    display: flex;
    flex-direction: column;
    font-family: Roboto, sans-serif;
    height: 100%;
    justify-content: center;
  }

  .app-container {
    color: #2c3e50;
    margin-top: -30vh;
    width: 75vw;

    h1 {
      text-align: center;
    }
  }
</style>
