<script>
import Form from '@/components/Form.vue'

export default {
  name: 'Survey',
  components: {
    Form
  }
}
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
  height: 83vh;
  background-color: rgba(0, 0, 0, 0.7);
  padding: 20px 40px;
  margin-bottom: 70px;
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

@media only screen and (min-width: 768px) {
  /* For desktop: */
  .survey-form {
    width: 700px;
    margin: 0 auto;
    margin-bottom: 25px;
    height: 70vh;
  }
}
</style>