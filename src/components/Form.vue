<script>
export default {
  name: 'Form'
}
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

    <div class="form-wrapper">
      <label>Which best describes you?</label>
      <select name="role" required>
        <option disabled selected value>Select current role</option>
        <option value="student">Student</option>
        <option value="job">Full Time Job</option>
        <option value="other">Other</option>
      </select>
    </div>
    <!-- TODO - add an input text box if a user selects Other -->

    <div class="form-wrapper">
      <label>What is your favourite programming language?</label>
      <select name="language" required>
        <option disabled selected value>Select current language</option>
        <option value="javascript">Javascript</option>
        <option value="python">Python</option>
        <option value="kotlin">Kotlin</option>
        <option value="java">Java</option>
      </select>
    </div>

    <div class="form-wrapper">
      <label>What is your level of experience with the language?</label>
      <label>
        <input
          name="level-experience"
          value="beginner"
          type="radio"
          class="input-radio"
          checked
        />Beginner</label
      >
      <label>
        <input
          name="level-experience"
          value="intermediate"
          type="radio"
          class="input-radio"
        />Intermediate</label
      >

      <label
        ><input
          name="level-experience"
          value="advanced"
          type="radio"
          class="input-radio"
        />Advanced</label
      >
    </div>


    <div class="form-wrapper">
      <label>
        Select the area of interests for your language
        <span>(Check all that apply)</span>
      </label>

      <label
        ><input
          name="prefer"
          value="front-end-projects"
          type="checkbox"
          class="input-checkbox"
        />Front-end Projects</label
      >
      <label>
        <input
          name="prefer"
          value="back-end-projects"
          type="checkbox"
          class="input-checkbox"
        />Back-end Projects</label
      >
      <label
        ><input
          name="prefer"
          value="coding-challenges"
          type="checkbox"
          class="input-checkbox"
        />Coding Challenges</label
      >
      <label
        ><input
          name="prefer"
          value="data-structures-algorithms"
          type="checkbox"
          class="input-checkbox"
        />Data Structures and Algorithms</label
      >
      <label
        ><input
          name="prefer"
          value="creative-coding"
          type="checkbox"
          class="input-checkbox"
        />Creative Coding</label
      >
    </div>

        <div class="form-wrapper">
      <p>Feedback and ways to improve?</p>
      <textarea
        id="comments"
        class="input-textarea"
        name="comment"
        placeholder="Enter your comment here..."
      ></textarea>
    </div>

    <div class="form-wrapper">
      <button type="submit">
        Submit
      </button>
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
