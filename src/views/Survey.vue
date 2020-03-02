<template>
  <div class="wrapper">
    <div class="survey-header">
      Survey Form Header
    </div>

    <div class="survey-form">
      Survey Form Section
    </div>

  </div>
</template>

<script>
export default {
  name: 'Survey'
}
</script>

<style scoped>
/* Mobile First Approach */
.wrapper {
  display: flex;
  flex-direction: column;
}

.survey-header {
  width: 100%;
  height: 20vh;
  border: 1px solid red;
}

.survey-form {
  height: 80vh;
  border: 1px solid blue;
}
</style>