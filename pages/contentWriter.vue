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
        'Amrita has been ranked 8th among the top 100 content writers in India by Contracts and Freelance, a community for creative people. The list was curated after screening 3000+ content writers. She has written 100+ Technical blogs on Emerging technologies like AI, Big Data, ML, Data Analytics and much more.',
      topics: [
        'Content Writing (What,Who,Why and How)',
        ' Tools used in Content writing',
        '  How to get your first freelance client?',
        'Poster Designing',
        'Future of content writing and so on',
      ],
      mentorProfile: {
        name: ' Amrita Angappa',
        company: ' Associate consultant - iQuantM technologies',
        image:
          'https://spotknackcompanywebsite.s3.us-east-2.amazonaws.com/images/amrita.jpg',
        linkedInURL: 'https://www.linkedin.com/in/amrita-angappa-19011212b/',
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
