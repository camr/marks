<template>
  <div>
    <ui-textbox label="Passphrase" name="passphrase"
                placeholder="Your passphrase..."
                value={{ passphrase }}>
    </ui-textbox>

    <ui-button type="flat" color="primary"
               @click="decrypt">Decrypt</ui-button>
  </div>
</template>

<script type="text/ecmascript-6">
  export default {
    data () {
      return {
        passphrase: ''
      }
    },

    methods: {
      decrypt () {
        console.log('Decrypt library data')
        console.log(this.passphrase)
      }
    }
  }
</script>
