<template>
  <div class="wrapper">
    <div class="flex-row-center-space-even web-banner">
      <div class="flex-col-center">
        <h2 class="info-header">Mock Interview</h2>
        <p class="p-text text-center mt-10">
          Become confident by attending mock interviews.Get constructive
          feedback from Mock Interviews and improve
        </p>
        <div class="button-align">
          <a
            href="http://bit.ly/spotknack_interview"
            title="Spotknack's Mission 2021 : Student Registration"
            target="_blank"
            onclick="zforms_open_window(this.href, 648, 700); return false"
          >
            <button class="apply-button poppins-font">Apply</button></a
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
    <!-- <div class="body-content">
      <div class="box-content-body">
        <div class="box-content-finder flex-col-center">
          <h2 class="info-header">Mock Interview</h2>
          <p class="p-text text-center">
            Become confident by attending mock interviews.Get constructive
            feedback from Mock Interviews and improve
          </p>
          <div class="button-align">
            <a href="http://bit.ly/spotknack_interview"
              ><button class="button-box poppins-font">Apply here</button>
            </a>
          </div>
        </div>
        <div class="box-content-analysis">
          <div class="box-image">
            <img
              src="~assets/images/mock.svg"
              width="100%"
              height="100%"
              alt="skillanalysis"
            />
          </div>
        </div>
      </div>
    </div> -->

    <!-- Why mock Interview content -->
    <div class="feature-description">
      <h2 class="info-header">Why do Mock Interview with us</h2>
      <!-- Feature description -->
      <p class="feature-description-content text-center mt-10">
        We work in the Skill development and Hiring sector, students will get
        knowledge of companies hiring and technology trends during the mock
        interview process.
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
  </div>
</template>

<script>
export default {
  data() {
    return {
      items: [
        {
          header: 'Resume Preparation',
          description:
            'Get useful insights to prepare a resume to show your skills and works that suits with a job description you deserve. And let your resume speak and get you your dream job.',
          color: '#ffdc5a',
        },
        {
          header: 'Startup Aspirants',
          description:
            'Students willing to join a start-up will get a dedicated support to make yourself a team-player in budding start-up and to be in the part of their journey building great company.',
          color: '#ff7ce7',
        },
        {
          header: 'Constructive Feedback',
          description:
            'It serves as a guide to assist you in your further steps you take and steps to be taken. You get a strong satisfaction that’s possible because of feedbacks you get from Interviewer.',
          color: '#c9fd6a',
        },
        {
          header: 'Evaluation Form',
          description:
            'Get yourself evaluated with resume evaluation to find your resume spoilers and other irrelevant contents that kills your resume to catch eye’s of the recruiter.',
          color: '#5afffb',
        },
        {
          header: 'Feedback Form',
          description:
            ' ake home with you feedback form that points your resume spoilers and other future steps to be taken to be a quality product in the Job Market.',
          color: '#74d30b',
        },
        {
          header: 'Interview Experience',
          description:
            'Provides an opportunity to practice your interviewing skills in an environment similar to an actual interview and tests your confidence level.',
          color: '#ebb0f4',
        },
      ],
    }
  },
}
</script>
<style scoped>
.flex-row-center-space-even {
  margin: 11% 5% 15% 5%;
}

@media only screen and (min-width: 768px) and (max-width: 991px) {
  .flex-row-center-space-even {
    margin: 15% 5% 15% 5%;
  }
}
</style>
