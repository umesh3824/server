<template>
  <div class="hello">
    <p>{{ value }}</p>
    <qrcode-vue :value="value" :size="size" level="H" /><br />
    <!-- <button @onclick="generate_qr">Generate</button> -->
  </div>
</template>

<script>
import QrcodeVue from 'qrcode.vue'

export default {
    data() {
      return {
        value: '{"string":"classroom_1", "token": "dG9rZW4K"}',
        size: 300,
      }
    },
    components: {
      QrcodeVue,
    },
  }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
