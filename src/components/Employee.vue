
<template>
  <div>
      <h3>Employee: {{ message }}</h3>
      <!-- <button @click="updateMessage()">Click here to update</button> -->
  </div>
</template>

<script>
export default {
    data() {
        return {
            message: 'Hi I am Employee Component'
        }
    }
}
</script>

<style>

</style>