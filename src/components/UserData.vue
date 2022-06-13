<template>
  <form @submit.prevent="addUser">
    <div>
      <label>Username: </label>
      <input type="text" v-model="enteredUsername" />
    </div>
    <div>
      <label>Age: </label>
      <input type="number" v-model="enteredAge" />
    </div>
    <button type="submit">Submit</button>
  </form>
</template>

<script>
export default {
  emits: ["user-submit"],
  data() {
    return {
      enteredUsername: "",
      enteredAge: "",
    };
  },
  methods: {
    addUser() {
      this.$emit("user-submit", this.enteredUsername, this.enteredAge);
      this.enteredUsername = "";
      this.enteredAge = "";
    },
  },
};
</script>
