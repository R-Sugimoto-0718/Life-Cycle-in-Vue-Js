<template>
  <div id="app">
    <student></student>
    <employee></employee>
    <h3>{{ sinpleText }}</h3>
    <button @click="updateMessage()">Click here to update</button>
  </div>
</template>

<script>
import Student from "./components/Student";
import Employee from "./components/Employee";

export default {
  components: {
    student: Student,
    employee: Employee
  },
  data() {
    return {
      sinpleText: "Simple text"
    };
  },
  methods: {
    updateMessage: function() {
      this.sinpleText = "Message has been updated";
    }
  },
  beforeCreate() {
    alert("Before Create");
  },
  created() {
    alert("Created");
  },
  beforeMount() {
    alert("Before mount");
  },
  mounted() {
    alert("Mounted");
  },
  beforeUpdate() {
    alert("Before update");
  },
  updated() {
    alert("updated ");
  }
};
</script>

<style>
</style>
