<template>
  <div class="wrapper">
    <div class="flex-row-center-space-even">
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
            <button class="button-box poppins-font">Apply</button></a
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
        <div class="feature-cluster" style="background-color: #ffdc5a">
          <h3 class="sub-header-H3">Resume Preparation</h3>

          <p class="feature-description-content">
            Get useful insights to prepare a resume to show your skills and
            works that suits with a job description you deserve. And let your
            resume speak and get you your dream job.
          </p>
        </div>
        <div class="feature-cluster" style="background-color: #ff7ce7">
          <h3 class="sub-header-H3">Startup Aspirants</h3>
          <p class="feature-description-content">
            Students willing to join a start-up will get a dedicated support to
            make yourself a team-player in budding start-up and to be in the
            part of their journey building great company.
          </p>
        </div>
        <div class="feature-cluster" style="background-color: #c9fd6a">
          <h3 class="sub-header-H3">Constructive Feedback</h3>
          <p class="feature-description-content">
            It serves as a guide to assist you in your further steps you take
            and steps to be taken. You get a strong satisfaction that’s possible
            because of feedbacks you get from Interviewer.
          </p>
        </div>
        <div class="feature-cluster" style="background-color: #5afffb">
          <h3 class="sub-header-H3">Evaluation Form</h3>
          <p class="feature-description-content">
            Get yourself evaluated with resume evaluation to find your resume
            spoilers and other irrelevant contents that kills your resume to
            catch eye’s of the recruiter.
          </p>
        </div>
        <div class="feature-cluster" style="background-color: #74d30b">
          <h3 class="sub-header-H3">Feedback Form</h3>
          <p class="feature-description-content">
            Take home with you feedback form that points your resume spoilers
            and other future steps to be taken to be a quality product in the
            Job Market.
          </p>
        </div>
        <div class="feature-cluster" style="background-color: #ebb0f4">
          <h3 class="sub-header-H3">Interview Experience</h3>
          <p class="feature-description-content">
            Provides an opportunity to practice your interviewing skills in an
            environment similar to an actual interview and tests your confidence
            level
          </p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {}
</script>
<style scoped>
.flex-row-center-space-even {
  margin: 7.6% 5%;
}

.flex-col-center {
  margin-right: 5%;
  width: 60%;
}
.button-box {
  width: 229px;
  height: 59px;
  border-radius: 8px;
  background-color: #c9fd6a;
  text-align: center;
  justify-content: center;
  font-size: 16px;
  color: black;
  font-weight: normal;
  font-style: normal;
  font-stretch: normal;
  line-height: normal;
  letter-spacing: 0.6px;
  border-style: none;
}
.body-content {
  display: flex;
  flex-direction: column;
}
.p-text {
  line-height: 1.75;
}
.box-content-body {
  display: flex;
  flex-direction: row;
  justify-content: center;
  width: 100%;
  padding: 5.5% 5% 0 5%;
}
.box-content-find {
  display: flex;
  flex-direction: row-reverse;
  justify-content: center;
  width: 90%;
  padding: 10% 5% 0 5%;
}
.box-content-page {
  display: flex;
  flex-direction: row;
  padding-left: 5%;
}
.box-content-finder {
  width: 40%;
  letter-spacing: 0.6px;
  line-height: 40px;
  padding-top: 5%;
}
.feature-description h2 {
  padding: 0 8.1%;
}
.feature-container {
  margin: 22% 0 8% 5.4%;
}
.feature-container h2 {
  margin-left: 1.8%;
  margin-bottom: 50px;
}
.feature-container .feature-cluster {
  width: 28.2%;
  margin: 0 4.7% 44px 0;
  border-radius: 10px;
  padding: 2.63% 2.93%;
}
.feature-cluster .feature-description-content {
  opacity: 0.7;
}
.box-content-page .box-content-finder {
  width: 30%;
  padding-left: 15%;
}
.box-content-analysis {
  width: 50%;
  padding-left: 10%;
  max-height: 352px;
}
.feature-description {
  width: 66%;
  margin: auto;
  margin-top: 10%;
}
@media screen and (max-width: 768px) {
  .box-content-body {
    flex-direction: column-reverse;
    align-items: center;
  }
  .box-content-analysis {
    width: auto;
    padding: 0;
  }
  .box-content-finder {
    width: 100%;
  }
  .feature-description {
    width: 80%;
    margin-top: 10%;
  }
  .feature-description h2 {
    padding: 0;
  }
}
@media only screen and (max-width: 640px) {
  .feature-container .feature-cluster {
    width: auto;
  }
  .flex-wrap {
    flex-direction: column;
  }
  .box-content-analysis {
    padding: 0;
  }
  .flex-row-center-space-even {
    flex-direction: column-reverse;
  }
  .flex-col-center {
    width: 80%;
    margin: auto;
  }
}
</style>
