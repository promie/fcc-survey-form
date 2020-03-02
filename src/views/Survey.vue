<template>
  <div class="wrapper">
    <div class="survey-header">
      Promie Survey Form
    </div>

    <div class="survey-form">

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
  background-color: red;
}

.survey-form {
  background-color: gray;
  height: 80vh;
}
</style>