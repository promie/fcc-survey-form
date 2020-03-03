<script>
import Form from "@/components/Form.vue";

export default {
  name: "Survey",
  components: {
    Form
  }
};
</script>

<template>
  <div class="wrapper">
    <div class="survey-header">
      <div class="title-header">Programming Survey Form</div>
      <div class="title-description">Thank you so much for taking the time to complete this survey!</div>
    </div>

    <div class="survey-form">
      <Form />
    </div>
  </div>
</template>

<style scoped>
/* Mobile First Approach */
.wrapper {
  display: flex;
  flex-direction: column;
}

.survey-header {
  width: 100%;
  height: 20vh;
}

.survey-form {
  height: 80vh;
  background-color: rgba(0, 0, 0, 0.7);
  border-radius: 10px;
}

.title-header {
  color: white;
  text-align: center;
  padding-top: 45px;
  font-size: 30px;
}

.title-description {
  color: white;
  text-align: center;
}
</style>