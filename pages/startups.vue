<template>
  <div class="wrapper">
    <div class="flex-row-center-space-even web-banner">
      <div class="flex-col-center">
        <h2 class="info-header">Hire Students With Us</h2>
        <p class="p-text text-center mt-10">
          Get Access To Skill Database of Students and Colleges
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

    <div class="feature-description">
      <h2 class="info-header">Why Hire Freshers With Us</h2>
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
          header: 'Post Internship',
          description:
            'Students are the best talent source for start-ups to get their content, development, marketing works, etc works done and accelerating with contribution and efforts. Just post internships and we take care of taking it to students.',
          color: '#ffdc5a',
        },
        {
          header: 'LeaderBoard',
          description:
            'Get pre-assessed profiles to accelerate your intern hiring or interview time by selecting students who top in the leader board scores from Spotknack assessment, of skills you choose or prefer.',
          color: '#ff7ce7',
        },
        {
          header: 'Role Configuration',
          description:
            'Attracting efficient talents will also require details like roles and respective skills you look for from students make them available to students to understand and equip skills by themselves.',
          color: '#c9fd6a',
        },
        {
          header: 'Recommended profiles',
          description:
            'Get good and skilled students profiles that you might have missed or you might need that Spotknack recommends by assessing those profiles personally to your dashboard.',
          color: '#5afffb',
        },
        {
          header: 'Employee Referrals',
          description:
            ' Employee referrals are the most used preferred medium of hiring for most start-ups, and here we got a solution for your employees to recommend or refer their college juniors profiles.',
          color: '#74d30b',
        },
        {
          header: 'Skill Profile',
          description:
            'Students tend to add unnecessary and irrelevant details to their resumes that don’t match a respective job description that might pressure in choosing best, but Spotknack gives you what you need by skill profile.',
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
@media only screen and (min-width: 768px) and (max-width: 991px) {
  .wrapper {
    margin: 15% 5% 15% 5%;
  }
}
</style>
