<template>
  <div class="htmlClass">
    <h1>{{ head }}</h1>
    <form>
      <input type="text" id="firstName" v-model="firstName" />
      <input type="text" id="secondName" v-model="secondName" />
      <input type="text" id="Codename" v-model="Codename" />
      <input type="text" id="nickname" v-model="nickname" />
      <button @click="submitForm()" class="submitForm">Submit</button>
  </form>
  </div>
</template>

<script>
export default {
  name: 'InputPage',
  data() {
    return {
      head: 'Vue is awesome.',
      firstName: 'นายกิตติคุณ',
      secondName: 'กิจวิบูลย์สิน',
      Codename:'6604101307',
      nickname:'เฮ็ฟเว่น',
    }
  },
  methods: {
    submitForm() {
      this.$emit('submit form')
    },
  }
}
</script>

<style scoped></style>