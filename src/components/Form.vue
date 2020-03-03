<script>
export default {
  name: "Form"
};
</script>

<template>
  <form id="survey-form">
    <div class="form-wrapper">
      <label for="name" class="title-spacer">Name</label>
      <input type="text" name="name" id="name" placeholder="Enter your name" required />
    </div>

    <div class="form-wrapper">
      <label for="email" class="title-spacer">Email</label>
      <input type="email" name="email" id="email" placeholder="Enter your name" required />
    </div>

    <div class="form-wrapper">
      <label for="age" class="title-spacer">Age (optional)</label>
      <input type="number" name="age" id="age" placeholder="Age" required />
    </div>

    <div class="form-wrapper">
      <div class="title-spacer">Which best describes you?</div>
      <select name="role" required>
        <option disabled selected value>Select current role</option>
        <option value="student">Student</option>
        <option value="job">Full Time Job</option>
        <option value="other">Looking For Work</option>
      </select>
    </div>

    <div class="form-wrapper">
      <div class="title-spacer">What is your favourite programming language?</div>
      <select name="language" required>
        <option disabled selected value>Select current language</option>
        <option value="javascript">Javascript</option>
        <option value="python">Python</option>
        <option value="kotlin">Kotlin</option>
        <option value="java">Java</option>
      </select>
    </div>

    <div class="form-wrapper">
      <div class="title-spacer">What is your level of experience with the language?</div>
      <label class="selection-label">
        <input name="level-experience" value="beginner" type="radio" checked />Beginner
      </label>
      <label class="selection-label">
        <input name="level-experience" value="intermediate" type="radio" />Intermediate
      </label>

      <label class="selection-label">
        <input name="level-experience" value="advanced" type="radio" />Advanced
      </label>
    </div>

    <div class="form-wrapper">
      <div class="title-spacer">
        Select the area of interests for your language
        <span>(Check all that apply)</span>
      </div>

      <label class="selection-label">
        <input name="prefer" value="front-end-projects" type="checkbox" />Front-end Projects
      </label>
      <label class="selection-label">
        <input name="prefer" value="back-end-projects" type="checkbox" />Back-end Projects
      </label>
      <label class="selection-label">
        <input name="prefer" value="coding-challenges" type="checkbox" />Coding Challenges
      </label>
      <label>
        <input
          name="prefer"
          value="data-structures-algorithms"
          type="checkbox"
          class="input-checkbox"
        />Data Structures and Algorithms
      </label>
      <label class="selection-label">
        <input name="prefer" value="creative-coding" type="checkbox" />Creative Coding
      </label>
    </div>

    <div class="form-wrapper">
      <div class="title-spacer">Feedback and ways to improve?</div>
      <textarea
        id="comments"
        class="input-textarea"
        name="comment"
        placeholder="Enter your comment here..."
      ></textarea>
    </div>

    <div class="form-wrapper">
      <button type="submit">Submit</button>
    </div>
  </form>
</template>

<style scoped>
.form-wrapper {
  color: white;
  margin-top: 10px;
}

input[type="text"],
input[type="email"],
input[type="number"] {
  width: 100%;
}

textarea {
  width: 100%;
  height: 200px;
}

select {
  width: 100%;
}

.selection-label {
  display: block;
}

.title-spacer {
  margin-bottom: 5px;
}
</style>
