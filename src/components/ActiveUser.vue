<template>
  <div>
    <h2><strong>Username: </strong>{{ username }}</h2>
    <h3><strong>Age: </strong>{{ age }}</h3>
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
