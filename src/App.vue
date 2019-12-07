<template>
  <div id="app">
    <student></student>
    <employee></employee>
  </div>
</template>

<script>
import Student from './components/Student'
import Employee from './components/Employee'

export default {
  components: {
    "student": Student,
    "employee": Employee
  },
 data() {
   return {
     
   }
 },
 beforeCreate() {
   alert('Before Create')
 },
 created() {
   alert('Created')
 },
 beforeMount() {
   alert("Before mount")
 }
}
</script>

<style>

</style>
