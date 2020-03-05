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
      <h1 class="title-header" id="title">Programming Survey Form</h1>
      <p
        class="title-description"
        id="description"
      >Thank you so much for taking the time to complete this survey!</p>
    </div>

    <div class="survey-form">
      <Form />
    </div>
  </div>
</template>

<style scoped>
@import url("https://fonts.googleapis.com/css?family=Fredoka+One&display=swap");
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
  height: 100%;
  background-color: rgba(0, 0, 0, 0.7);
  padding: 20px 40px;
  margin-bottom: 70px;
  border-radius: 6px;
}

.title-header {
  color: lightskyblue;
  text-align: center;
  padding-top: 25px;
  font-size: 25px;
  font-family: "Fredoka One", cursive;
}

.title-description {
  color: white;
  text-align: center;
  font-size: 16px;
  margin-top: -17px;
}

@media only screen and (min-width: 768px) {
  /* For desktop: */
  .survey-form {
    width: 700px;
    margin: 0 auto;
    margin-bottom: 25px;
    height: 100%;
    font-size: 16px;
  }
  .title-header {
    font-size: 35px;
    padding-top: 10px;
  }
  .title-description {
    font-size: 20px;
    margin-top: -25px;
  }
}
</style>