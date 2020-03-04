<script>
import { ROLES, LANGUAGES, EXPERIENCES, PREFERENCES } from '@/constants'

export default {
  name: 'Form',
  data() {
    return {
      roles: ROLES,
      languages: LANGUAGES,
      experiences: EXPERIENCES,
      preferences: PREFERENCES
    }
  }
}
</script>

<template>
  <form id="survey-form">
    <div class="form-wrapper">
      <label for="name" class="title">Name</label>
      <input type="text" name="name" id="name" placeholder="Enter your name" required />
    </div>

    <div class="form-wrapper">
      <label for="email" class="title">Email</label>
      <input type="email" name="email" id="email" placeholder="Enter your name" required />
    </div>

    <div class="form-wrapper">
      <label for="age" class="title">Age (optional)</label>
      <input type="number" name="age" id="age" placeholder="Age" required />
    </div>

    <div class="form-wrapper">
      <div class="title">Which best describes you?</div>
      <select name="role" required>
        <option disabled selected value>Select current role</option>
        <option v-for="role in roles" v-bind:key="role.id" value="role.id">{{ role.desc }}</option>
      </select>
    </div>

    <div class="form-wrapper">
      <div class="title">What is your favourite programming language?</div>
      <select name="language" required>
        <option disabled selected value>Select current language</option>
        <option v-for="lang in languages" v-bind:key="lang.id" value="lang.id">{{ lang.desc }}</option>
      </select>
    </div>

    <div class="form-wrapper">
      <div class="title">What is your level of experience with the language?</div>
      <label class="selection-label" v-for="experience in experiences" v-bind:key="experience.id">
        <input name="level-experience" value="experience.id" type="radio" />{{ experience.desc }}
      </label>
    </div>

    <div class="form-wrapper">
      <div class="title">
        Select the area of interests for your language
        <span>(Check all that apply)</span>
      </div>
      <label class="selection-label" v-for="preference in preferences" v-bind:key="preference.id">
        <input name="prefer" value="preference.id" type="checkbox" />{{ preference.desc }}
      </label>
    </div>

    <div class="form-wrapper">
      <div class="title">Feedback and ways to improve?</div>
      <textarea
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

input[type='text'],
input[type='email'],
input[type='number'] {
  width: 100%;
}

textarea {
  width: 100%;
  height: 80px;
}

select {
  width: 100%;
}

.selection-label {
  display: block;
}

.title {
  font-weight: 900;
  color: lightskyblue;
}

@media only screen and (min-width: 768px) {
  /* For desktop: */
  text-area {
    height: 50px;
  }

  .title {
    font-size: 16px;
  }
}
</style>
