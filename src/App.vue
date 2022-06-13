<template>
  <active-user
    v-for="user in users"
    :key="user.id"
    :id="user.id"
    :username="user.name"
    :age="user.age"
  ></active-user>
</template>

<script>
export default {
  data() {
    return {
      users: [
        {
          id: "Supakit",
          name: "Supakit",
          age: 28,
        },
      ],
    };
  },
};
</script>
