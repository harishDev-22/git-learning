<template>
  <div class="wrapper">
    <div class="flex-row-center-space-even web-banner">
      <div class="flex-col-center">
        <h2 class="info-header">Connect With Your Students</h2>
        <p class="p-text text-center mt-10">
          Access , Track Performance and Mentor them To Reach Heights
        </p>
        <div class="button-align">
          <a
            href="#"
            title="Spotknack's Mission 2021 : Student Registration"
            target="_blank"
            onclick="zforms_open_window(this.href, 648, 700); return false"
          >
            <button class="apply-button poppins-font">
              Apply Here For Early Access
            </button></a
          >
        </div>
      </div>

      <img
        class="mentoring-images"
        src="~assets/images/mock.svg"
        width="100%"
        height="100%"
        alt="skillanalysis"
      />
    </div>

    <!-- Why Engage Students With Us -->
    <div class="feature-description">
      <h2 class="info-header">Why Engage Students With Us</h2>
      <!-- Feature description -->
      <p class="feature-description-content text-center mt-10">
        The vision of spotknack is to bridge students and employers in a common
        platform, where both students and employers get involved in an indirect
        conversation to exchange skills and requirements respectively.
      </p>
    </div>

    <!-- Feature benefits  -->
    <div class="feature-container">
      <h2 class="sub-header-H2 text-left">What benefits you would get</h2>
      <div class="flex-wrap">
        <div
          v-for="(item, $index) in items"
          :key="$index"
          class="feature-cluster"
          :style="{ backgroundColor: item.color }"
        >
          <h3 class="sub-header-H3">{{ item.header }}</h3>
          <p class="feature-description-content">
            {{ item.description }}
          </p>
        </div>
      </div>
    </div>

    <!-- Appication form -->
    <div class="form-group-block">
      <b-form v-if="show" @submit="onSubmit" @reset="onReset">
        <h2 class="sub-header-H3">
          Get Access to our Platform ! Enter your details here !
        </h2>
        <!-- Name -->
        <b-form-group id="input-group-1">
          <b-form-input
            id="input-1"
            v-model="form.email"
            type="email"
            placeholder="Enter name"
            required
          ></b-form-input>
        </b-form-group>
        <!-- Email -->
        <b-form-group id="input-group-2">
          <b-form-input
            id="input-2"
            v-model="form.name"
            placeholder="Enter Email"
            required
          ></b-form-input>
        </b-form-group>

        <!-- College Name -->
        <b-form-group id="input-group-3">
          <b-form-input
            id="input-3"
            v-model="form.name"
            placeholder="Enter college name"
            required
          ></b-form-input>
        </b-form-group>

        <!-- College Website -->
        <b-form-group id="input-group-4">
          <b-form-input
            id="input-4"
            v-model="form.name"
            placeholder="Enter College Website"
            required
          ></b-form-input>
        </b-form-group>
        <!-- MobileNumber -->
        <b-form-group id="input-group-5">
          <b-form-input
            id="input-5"
            v-model="form.name"
            placeholder="Mobile Number"
            required
          ></b-form-input>
        </b-form-group>
        <div class="flex-row-center">
          <button class="form-button">Submit</button>
        </div>
      </b-form>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      items: [
        {
          header: 'Skill Profile',
          description:
            'Getting or collecting resumes of your student is no longer trouble; we build skill profile and make it available with the click of a button. And analyze your student performance on different skill sets based on the scores from assessments.',
          color: '#ffdc5a',
        },
        {
          header: 'LeaderBoard',
          description:
            ' Find from best to students who need help in improving their employability skills through the leader board ranking of scores obtained from our contests and assessments in your dashboard.',
          color: '#ff7ce7',
        },
        {
          header: 'Opportunities',
          description:
            'Getting to know the internship or job opportunities posted or available in the job market might have been tough to help your students, now all those posted by companies who use the Spotknack platform to hire students will be in your inbox.',
          color: '#c9fd6a',
        },
        {
          header: 'Recommend To Students',
          description:
            'With all opportunities available in your inbox, you can recommend the right internship to the right set of students by just entering their names.',
          color: '#5afffb',
        },
        {
          header: 'Recommend To Company',
          description:
            'Get Job or Internship for students who are hunting for the opportunities despite good skills, by sending or recommending the profile to companies.',
          color: '#74d30b',
        },
        {
          header: 'Associate With Students',
          description:
            'Enable and also restrict students to enroll or associate with your account by generating a random access id and sharing it with your students.',
          color: '#ebb0f4',
        },
      ],
      form: {
        email: '',
        name: '',
      },

      show: true,
    }
  },
  methods: {
    onSubmit(event) {
      event.preventDefault()
      alert(JSON.stringify(this.form))
    },
    onReset(event) {
      event.preventDefault()
      // Reset our form values
      this.form.email = ''
      this.form.name = ''
      this.form.food = null
      this.form.checked = []
      // Trick to reset/clear native browser form validation state
      this.show = false
      this.$nextTick(() => {
        this.show = true
      })
    },
  },
}
</script>
<style scoped>
.wrapper {
  margin: 11% 5% 15% 5%;
}

/* Application form  styles */
.form-group-block {
  width: 84%;
  max-width: 1060px;
  margin: auto;
  border-radius: 10px;
  background-color: #5afffb;
}
form {
  width: 73%;
  margin: auto;
  padding-top: 55px;
  padding-bottom: 55px;
}
.form-group {
  width: 55%;
  margin: auto;
  margin-top: 4%;
}
.form-control {
  border: none;
  border-radius: 10px;
}
.form-button {
  margin-top: 7.2%;
  width: 279px;
  height: 61px;
  border-radius: 10px;
  background-color: #131415;
  font-size: 24px;
  font-weight: normal;
  font-stretch: normal;
  font-style: normal;
  line-height: normal;
  letter-spacing: 0.8px;
  color: #fff;
}

@media only screen and (min-width: 768px) and (max-width: 991px) {
  .wrapper {
    margin: 15% 5% 15% 5%;
  }
}
@media only screen and (max-width: 1024px) {
  .form-group {
    width: 75%;
  }
}
@media screen and (max-width: 768px) {
  form {
    width: 90%;
  }
  .form-group {
    width: 100%;
  }
  .form-button {
    height: 50px;
  }
}
</style>
