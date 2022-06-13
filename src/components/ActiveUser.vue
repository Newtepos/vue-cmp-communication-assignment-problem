<template>
  <div>
    <div><strong>Username: </strong>{{ username }}</div>
    <div><strong>Age: </strong>{{ age }}</div>
  </div>
</template>

<script>
export default {
  props: {
    id: {
      type: String,
      required: true,
    },
    username: {
      type: String,
      required: true,
    },
    age: {
      type: Number,
      required: true,
    },
  },
};
</script>
