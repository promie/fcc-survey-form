<script>
export default {
  name: "Form"
};
</script>

<template>
  <form id="survey-form">
    <div class="form-wrapper">
      <label for="name">Name</label>
      <input type="text" name="name" id="name" placeholder="Enter your name" required />
    </div>

    <div class="form-wrapper">
      <label for="email">Email</label>
      <input type="email" name="email" id="email" placeholder="Enter your name" required />
    </div>

    <div class="form-wrapper">
      <label for="age">Age (optional)</label>
      <input type="number" name="age" id="age" placeholder="Age" required />
    </div>
  </form>
</template>

<style scoped>
.form-wrapper {
  color: white;
}

label {
  display: block;
}

input {
  width: 100%;
}
</style>
