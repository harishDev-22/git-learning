<template>
  <div class="wrapper">
    <h2 class="sub-header-H2 text-left">Program Details</h2>
    <div class="flex-row-center-space-bw">
      <mentoringProgramDescription />
      <!-- button -->
      <a
        class="button-block"
        href="http://bit.ly/spotknack_interview"
        title="Spotknack's Mission 2021 : Student Registration"
        target="_blank"
        onclick="zforms_open_window(this.href, 648, 700); return false"
      >
        <button class="apply-button poppins-font">Apply</button></a
      >
    </div>
    <mentoringProgram-aboutMentor
      :description="aboutMentorDescription"
      :topiclist="topics"
      :mentorprofile="mentorProfile"
    />
  </div>
</template>

<script>
export default {
  data() {
    return {
      aboutMentorDescription:
        "  Balakrishnan is self-taught Android App Developer with 3 years' experience. Worked on diverse project from Real time chat to Video streaming apps. Develops apps for Mobile, Tablet, and TV. Focus more onPixel perfection and quality of the product.",
      topics: [
        'Activity , Fragment , Services',
        'Views',
        ' Local Database',
        'Notifications',
        'Working With API and so on',
      ],
      mentorProfile: {
        name: 'Bala Krishnan',
        company: ' Android App Developer - Spectrum Global, Singapore',
        image:
          'https://spotknackcompanywebsite.s3.us-east-2.amazonaws.com/images/balakrishnan.jpg',
        linkedInURL: 'https://www.linkedin.com/in/balakrishnanpt/',
      },
    }
  },
}
</script>

<style scoped>
.wrapper {
  margin: 14.51% 8.3% 14.51% 4.9%;
}

@media only screen and (min-width: 2000px) {
  .wrapper {
    margin-top: 100px !important;
  }
}
@media only screen and (max-width: 991px) {
  .flex-row-center-space-bw {
    flex-direction: column;
    justify-content: center;
  }
  .program-description,
  .button-block {
    width: auto;
  }
  .button-block {
    margin-top: 50px;
  }
}
</style>
