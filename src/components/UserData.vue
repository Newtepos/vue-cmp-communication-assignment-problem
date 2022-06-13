<template>
  <form @submit.prevent="">
    <div>
      <label>Username: </label>
      <input type="text" />
    </div>
    <div>
      <label>Age: </label>
      <input type="number" />
    </div>
    <button type="submit">Submit</button>
  </form>
</template>

<script>
export default {};
</script>
