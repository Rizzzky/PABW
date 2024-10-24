<template>
  <div>
    <input type="number" v-model="bilangan1" placeholder="Isikan Bilangan 1">
    +
    <input type="number" v-model="bilangan2" placeholder="Isikan Bilangan 2">
    =
    <input type="number" :value="hasil" disabled>
    <button @click="hitung">HITUNG</button>
  </div>
</template>

<script>
export default {
  data() {
    return {
      bilangan1: 0,
      bilangan2: 0,
      hasil: 0
    }
  },
  methods: {
    hitung() {
      this.hasil = this.bilangan1 + this.bilangan2;
    }
  }
}
</script>
