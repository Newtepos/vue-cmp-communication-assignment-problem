<template>
  <user-data></user-data>
  <active-user
    v-for="user in users"
    :key="user.id"
    :id="user.id"
    :username="user.name"
    :age="user.age"
  ></active-user>
</template>

<script>
import UserData from "./components/UserData.vue";
export default {
  components: { UserData },
  data() {
    return {
      users: [
        {
          id: "Supakit",
          name: "Supakit",
          age: 27,
        },
      ],
    };
  },
};
</script>
