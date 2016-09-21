<template>
  <ui-textbox label="Passphrase" name="passphrase"
              placeholder="Your passphrase..."
              :value.sync="passphrase" :type.sync="inputType"
              @focussed="focusPassphrase">
  </ui-textbox>

  <div class="actions">
    <ui-button type="flat" color="primary" raised
               @click="decrypt">Decrypt</ui-button>
  </div>
</template>

<script type="text/ecmascript-6">
  export default {
    data () {
      return {
        passphrase: '',
        inputType: 'text'
      }
    },

    methods: {
      decrypt () {
        console.log('Decrypt library data')
        console.log(this.passphrase)
        this.inputType = 'password'
      },

      focusPassphrase () {
        this.inputType = 'text'
      }
    }
  }
</script>

<style lang="scss" scoped>
  .actions {
    text-align: right;
  }
</style>
