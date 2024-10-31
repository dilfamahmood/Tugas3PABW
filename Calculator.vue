<template>
  <div class="calculator">
    <input type="text" v-model="num1" placeholder="Masukkan angka pertama">
    <input type="text" v-model="num2" placeholder="Masukkan angka kedua">
    <button @click="hitung">Hitung</button>
    <p>Hasil: {{ hasil }}</p>
  </div>
</template>

<script>
export default {
  data() {
    return {
      num1: '',
      num2: '',
      hasil: ''
    }
  },
  methods: {
    hitung() {
      this.hasil = parseFloat(this.num1) + parseFloat(this.num2);
    }
  }
}
</script>
