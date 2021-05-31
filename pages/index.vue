<template>
  <div class="home-page-container">
    <!-- Initial youtube video -->
    <div v-if="infoVideo" id="video-container">
      <h3 class="youtube-video-heading">Spotknack's Mission 2021</h3>
      <div id="close-button" @click="closeInfoVideo">
        <img src="~assets/images/close-circle.svg" alt="" />
      </div>
      <!-- The src link contains 
                (enablejsapi=1)==youtube iframe api
                (autoplay=1)==autoplay the video
                (mute=1)==video starts with mute state 
                -->
      <iframe
        id="iframe-youtube-video"
        class="ad-video"
        width="50%"
        height="100%"
        src="https://www.youtube.com/embed/CZmxMZNVnDk?enablejsapi=1&autoplay=1&mute=1"
        allowFullScreen="allowFullScreen"
      ></iframe>
      <div class="youtube-video-linking-button">
        <a
          href="https://zfrmz.com/S2sA7QcE5hJbjsbmXnbT?referrername=spotknackvideo"
          >Student Registration</a
        >
      </div>
    </div>
    <!--header , replace the content with the respective text-->
    <div class="header">
      <div class="header-content">
        We help Students find skills and Companies find Students
      </div>
    </div>
    <!--sub heading , replace the content with the text -->
    <div class="subheader">
      <div class="subheader-content">
        <p>
          Let's make learning fun for the students. Let the students race
          through the various levels, solve nerve racking engineering
          problems,upgrade their skills, earn points and connect with potential
          recruiters .
        </p>
      </div>
    </div>
    <!-- /* trusted company */ -->
    <div class="customer">
      <span>Company who trust us</span>
      <img src="~assets/images/facilio.png" width="100" alt="facilio logo" />
    </div>

    <!--features -->
    <div class="body-box">
      <h1>If you are a student</h1>
      <div class="box-content">
        <div class="box-finder box-col1">
          <h2>Skill Analysis</h2>
          <p>
            Analyses the progress in your skillset by tracking your performance
            and recommends further steps,
          </p>

          <!---<h2><a href="features.html">Read more &#8594;</a></h2> -->
        </div>
        <div class="box-finder box-col2">
          <h2>Leaderboard</h2>
          <p>
            Ranks students based on specific skills. Use the sort option to
            filter the list as per your.
          </p>
          <!---      <h2><a href="features.html">Read more &#8594;</a></h2> -->
        </div>
        <div class="box-finder box-col3">
          <h2>Opportunities</h2>
          <p>
            Apply for Internship and Job Opportunities just by click of a
            Button.
          </p>

          <!--- <h2><a href="features.html">Read more &#8594;</a></h2> -->
        </div>
      </div>
      <!--sec row box -->
      <div class="box-content home-video-container2">
        <div class="box-test">
          <h2>Add Skills</h2>
          <p>
            Let’s you update your newly acquired skills and helps you get
            featured.
          </p>
          <!----   <h2><a href="features.html">Read more &#8594;</a></h2> -->
        </div>
        <!--video -->
        <div id="video-box-container" class="box-video-content">
          <div class="paragraph playfair-font">
            <p>See how it Works!</p>
          </div>
          <div
            id="workflow-video-parent"
            class="video_con"
            @click="showStudentMissionVideo"
          >
            <iframe
              id="workflow-student-video"
              class="frame"
              width="230"
              height="230"
              onclick="iframeclick()"
              src="https://www.youtube.com/embed/joat68b10y0?enablejsapi=1&autoplay=0&mute=1"
              allowFullScreen="allowFullScreen"
            ></iframe>
          </div>
        </div>
      </div>
    </div>

    <!--features-company-->
    <div class="body-box body-box-company">
      <h1>If you are a Company</h1>
      <div class="box-content">
        <div class="box-finder box-col1">
          <h2>Post Internship</h2>
          <p>
            Students are the best talent source for start-ups to get their
            content, development, marketing works, etc,
          </p>
          <h2><a href="views/startups.html">Read more &#8594;</a></h2>
        </div>
        <div class="box-finder box-col2">
          <h2>LeaderBoard</h2>
          <p>
            Get pre-assessed profiles to accelerate your intern hiring or
            interview time by selecting students who top,
          </p>
          <h2><a href="views/startups.html">Read more &#8594;</a></h2>
        </div>
        <div class="box-finder box-col3">
          <h2>Role Configuration</h2>
          <p>
            Attracting efficient talents will also require details like roles
            and respective skills you look,
          </p>
          <h2><a href="views/startups.html">Read more &#8594;</a></h2>
        </div>
      </div>
      <!--sec row box-->
      <div class="box-content home-video-container2">
        <div class="box-test">
          <h2>Employee Referrals</h2>
          <p>
            Employee referrals are the most used preferred medium of hiring for
            most start-ups,
          </p>
          <h2><a href="views/startups.html">Read more &#8594;</a></h2>
        </div>
        <!--video-->
        <div class="box-video-content-company">
          <div class="paragraph">
            <p>See how it Works!</p>
          </div>
          <div class="video_con" @click="showCompanyMissionVideo">
            <iframe
              id="workflow-company-video"
              class="frame"
              width="230"
              height="230"
              src="https://www.youtube.com/embed/xi6GR070TCI?enablejsapi=1&autoplay=0&mute=1"
              frameborder="2"
              allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture"
              allowfullscreen
            ></iframe>
          </div>
        </div>
      </div>
    </div>

    <!-- testimonial -->
    <div class="slider">
      <div class="slide">
        <div class="image-slider">
          <!---      <div class="image-test">
                    <a href="https://facilio.com" target="blank"> <img src="images/facilio.png" alt="facailio logo" width="100" height="100"> </a>
                </div> -->

          <p class="poppins-font">
            <mark class="quote">“</mark>I see this as a step to bigger and
            better things. Being a part of Spotknack I have learned a lot and
            planned my career path in a perfect way.
          </p>
        </div>
        <div class="image-slider">
          <div class="image-test">
            <img
              style="border-radius: 50%"
              src="https://spotknackcompanywebsite.s3.us-east-2.amazonaws.com/images/deepthi.jpg"
              alt="Nivedhitha"
              width="100"
              height="100"
            />
          </div>
          <p class="poppins-font">
            I like working with same mind people to still improve my skills and
            also showcase my talents in all the ways.<mark class="invert"
              >&#8217;&#8217;</mark
            >
          </p>
        </div>
      </div>
    </div>

    <div v-if="studentInfoVideo" id="student-video-container">
      <div id="close-button" @click="closeInfoVideo">
        <img src="~assets/images/close-circle.svg" alt="" />
      </div>
      <!-- The src link contains 
                (enablejsapi=1)==youtube iframe api
                (autoplay=1)==autoplay the video
                (mute=1)==video starts with mute state 
                -->
      <iframe
        id="iframe-youtube-video"
        class="ad-video"
        width="50%"
        height="100%"
        src="https://www.youtube.com/embed/joat68b10y0?enablejsapi=1&autoplay=1&mute=1"
        allowFullScreen="allowFullScreen"
      ></iframe>
    </div>
    <!--  video container for spotknack company mission -->
    <div v-if="companyInfoVideo" id="company-video-container">
      <div id="company-mission-video-stop" @click="closeInfoVideo">
        <img src="~assets/images/close-circle.svg" alt="" />
      </div>
      <iframe
        id="iframe-company-mission-video"
        class="ad-video"
        width="50%"
        height="100%"
        src="https://www.youtube.com/embed/xi6GR070TCI?enablejsapi=1&autoplay=1&mute=1"
        allowFullScreen="allowFullScreen"
      ></iframe>
    </div>
  </div>
</template>

<script>
export default {
  /* eslint-disable */
  data() {
    return {
      player: {},
      player2: {},
      player3: {},
      studentMissionVideo: {},
      companyMissionVideo: {},
      infoVideo: true,
      studentInfoVideo: false,
      companyInfoVideo: false,
    }
  },
  mounted() {
    // youtube iframe api
    //  these scripts added for to  avoid the autoplay restriction on mobile devices
    const tag = document.createElement('script')
    tag.id = 'iframe-demo'
    tag.src = 'https://www.youtube.com/iframe_api'
    const firstScriptTag = document.getElementsByTagName('script')[0]
    firstScriptTag.parentNode.insertBefore(tag, firstScriptTag)

    window.onYouTubeIframeAPIReady = () => {
      this.player = new YT.Player('iframe-youtube-video', {
        playerVars: { autoplay: 1, controls: 0 },
        events: {
          onReady: this.onPlayerReady,
        },
      })
    }
  },
  methods: {
    onPlayerReady(event) {
      event.target.playVideo()
    },
    stopVideo() {
      this.player.stopVideo()
    },
    showStudentMissionVideo() {
      this.companyInfoVideo = false
      this.studentInfoVideo = true
    },
    showCompanyMissionVideo() {
      this.companyInfoVideo = true
      this.studentInfoVideo = false
    },
    closeInfoVideo() {
      // this.stopVideo()
      this.infoVideo = false
      this.studentInfoVideo = false
      this.companyInfoVideo = false
    },
  },
}
</script>

<style>
.header {
  width: 100%;
  margin-top: 80px;
  display: flex;
  justify-content: center;
  text-align: center;
}

.header-content-index {
  padding-top: 5%;
  letter-spacing: 2px;
  font-size: 60px;
  text-align: center;
}

.header-content {
  padding-top: 5%;
  letter-spacing: 2px;
  font-size: 60px;
  font-weight: bold;
}

/*   sub heading under the header */

.subheader {
  display: flex;
  justify-content: center;
  padding-top: 0.5%;
}
.subheader-content {
  text-align: center;
  width: 50%;
  font-size: 1rem;
  letter-spacing: 0.6px;
  line-height: 1.75rem;
}

/* trusted company */
.customer {
  display: flex;
  flex-direction: row;
  justify-content: center;
  align-items: center;
}
.customer > img {
  margin-left: 2.1%;
}
.customer p {
  font-size: 1rem;
  padding-top: 2.5%;
  letter-spacing: 0.7px;
}

/* student progress  */
.body-box {
  width: 100%;
}
.body-box h1 {
  letter-spacing: 1.27px;
  padding: 0;
  padding-left: 10%;
  font-size: 2.375rem;
  font-weight: bold;
}
.body-box-company {
  margin-top: 55px;
}

.box-content {
  display: flex;
  width: 83%;
  margin: 20px 8.5% 20px 8.5%;
  padding: 0;
  word-break: break-word;
}
.box-content.home-video-container2 {
  display: flex;
  justify-content: space-between;
  width: 83%;
  margin: 20px 8.5% 20px 8.5%;
  padding: 0;
}

.box-content p {
  padding-left: 5%;
  letter-spacing: 0.6px;
  line-height: 1.75;
  font-size: 1rem;
  font-weight: normal;
  font-style: normal;
  font-stretch: normal;
  color: #000;
}

.box-content h2 {
  padding-left: 5%;
  letter-spacing: 0.93px;
  font-size: 1.75rem;
  font-weight: bold;
}
.box-content a {
  font-size: 1rem;
  font-weight: bold;
  font-style: normal;
  font-stretch: normal;
  line-height: 1.75;
  letter-spacing: 0.6px;
  text-decoration: none;
  color: #000;
}
.box-content-finder {
  flex-direction: row;
  flex-wrap: wrap;
  justify-content: space-around;
  width: 40%;
  letter-spacing: 0.6px;
  line-height: 40px;
  padding-top: 10%;
}

.flex-column {
  flex: 30%;
  padding: 10px;
}

.box-column {
  width: 18.75rem;
  height: 230px;
  border-radius: 10px;
  padding: 15px;
}
.box-col1 {
  background-color: #ffdc5a !important;
}
.box-col2 {
  background-color: #5afffb !important;
}
.box-col3 {
  background-color: #c9fd6a !important;
}
.box-content > .box-finder {
  margin: 0;
  margin-left: 1.4%;
  padding: 3.3% 3.6%;
  border-radius: 10px;
  width: 30%;
}
.box-content > .box-analysis {
  background-color: #5afffb;
  margin: 20px;
  padding: 30px;
  border-radius: 10px;
  width: 30%;
}
.box-content > .box-badges {
  background-color: #c9fd6a;
  margin: 20px;
  padding: 30px;
  border-radius: 10px;
  width: 30%;
}
.box-test {
  width: 30%;
  letter-spacing: 0.6px;
  text-align: justify;
}
.box-test-content {
  width: 30%;
  letter-spacing: 0.6px;
  text-align: justify;
}
.box-content > .box-test-content {
  background-color: #ff7ce7;
  margin: 20px;
  padding: 20px;
  border-radius: 10px;
}

.box-content > .box-test {
  background-color: #ff7ce7;
  margin: 0 1.4%;
  padding: 3.3% 3.6%;
  border-radius: 10px;
}

.box-content-body {
  display: flex;
  flex-direction: row;
  justify-content: center;
  width: 100%;
  padding: 10% 5% 0 5%;
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

.box-content-finder h2 {
  width: 499px;
  font-size: 60px;
  font-weight: bold;
  font-stretch: normal;
  font-style: normal;
  line-height: normal;
  letter-spacing: 2px;
  color: #000;
}

.box-content-page .box-content-finder {
  width: 30%;
  padding-left: 15%;
}
.box-content-analysis {
  width: 50%;
  padding-left: 10%;
}
.box-video-content-company {
  background-image: linear-gradient(
    to left,
    #d16ba5,
    #ef7386,
    #f78867,
    #eaa651,
    #ccc452,
    #b4d465,
    #98e281,
    #76eea3,
    #69f2b9,
    #5ff6cd,
    #5bf9e0,
    #5ffbf1
  );
  border-radius: 10px;
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: center;
  margin: 0;
  margin-right: 5.5%;
}
.box-video-content {
  background-image: linear-gradient(
    to left,
    #d16ba5,
    #ef7386,
    #f78867,
    #eaa651,
    #ccc452,
    #b4d465,
    #98e281,
    #76eea3,
    #69f2b9,
    #5ff6cd,
    #5bf9e0,
    #5ffbf1
  );
  border-radius: 10px;
  display: flex;
  flex-direction: row-reverse;
  padding: 1% 0% 0 0%;
  margin: 0;
  align-items: center;
  justify-content: center;
}
.home-video-container2 .box-video-content {
  margin-right: 5.5%;
}
.paragraph p {
  font-weight: bold;
  font-style: normal;
  font-stretch: normal;
  font-size: 3.75rem;
  color: white;
  letter-spacing: 2.17px;
  line-height: normal;
  text-shadow: 0 2px 34px rgba(0, 0, 0, 0.5);
}
.video_con {
  padding: 3% 5%;
}
.frame {
  border-radius: 50%;
  background-color: #00000f;
  background-image: url(~assets/images/s-tum.jpg);
  width: 230px;
  height: 230px;
  pointer-events: none;
}

.frame1 {
  border-radius: 50%;
  background-color: #00000f;
  background-image: url(~assets/images/c-tum.jpg);
  width: 230px;
  height: 230px;
}

.frame img {
  padding-top: 50px;
  padding-left: 15px;
}
.frame1 img {
  padding-top: 50px;
  padding-left: 15px;
}

/* testimoial styles */

.slider {
  text-align: center;
  overflow: hidden;
  font-size: 28px;
  padding: 170px 0 10% 15%;
}
.image-test {
  border-radius: 50%;
}
.quote {
  background: none;
  color: #b4d465;
  font-size: 6.25rem;
}
.invert {
  background: none;
  color: #ffdc5a;
  font-size: 100px;
  float: right;
}

.slide {
  width: 80%;
}
.slide p {
  font-size: 1.25rem;
  font-weight: normal;
  font-style: normal;
  font-stretch: normal;
  letter-spacing: 0.93px;
  text-align: center;
  line-height: 50px;
}
.image-slider p {
  width: 80%;
  padding: 0 0 0 10%;
}

.map p {
  margin-top: 20px;
}

/* testimoial styles */

/* --------index page youtube video modal----------- */

/* index page video container */

#video-container,
#student-video-container,
#company-video-container {
  width: 100%;
  height: 60vh;
  display: flex;
  justify-content: center;
  align-items: center;
  position: fixed;
  top: 25%;
  background: #fff;
  z-index: 10;
}
#mission-video-container__student,
#mission-video-container__company {
  width: 100%;
  height: 100vh;
  justify-content: center;
  align-items: center;
  background-color: #fff;
  display: none;
  position: fixed;
}

.youtube-video-heading {
  align-self: baseline;
  position: absolute;
  left: auto;
  text-align: center;
  width: 100%;
  height: 30px;
  background: #fff;
}
.youtube-video-linking-button {
  align-self: baseline;
  position: absolute;
  top: 100%;
  left: auto;
  text-align: center;
  width: 100%;
  background: #fff;
  height: 50px;
  justify-content: center;
  display: flex;
  align-items: center;
}
.youtube-video-linking-button a {
  text-decoration-line: none;
  color: black;
  text-align: center;
  font-weight: bold;
  width: auto;
  align-items: center;
  display: flex;
  justify-content: center;
  padding: 5px;
  height: 30px;
}
.youtube-video-linking-button a:hover {
  background-color: #c9fd6a;
}
#close-button,
#mission-video-stop,
#company-mission-video-stop {
  position: absolute;
  top: 5%;
  right: 5%;
  width: 50px;
  height: 50px;
  z-index: 10;
  background: white;
  border-radius: 50%;
}
#mission-video-stop:hover,
#company-mission-video-stop:hover,
#close-button:hover {
  cursor: pointer;
  border: 1px solid grey;
}

/* --------index page youtube video modal----------- */
@media only screen and (min-width: 320px) and (max-width: 640px) {
  .home-page-container {
    margin: 0 3%;
  }
  .box-finder,
  .box-analysis,
  .box-badges,
  .box-test,
  .box-video-content,
  .box-test-content,
  .box-content,
  .header {
    box-sizing: content-box;
  }
  .header {
    padding-top: 3%;
    width: 100%;
  }
  .header-content {
    text-align: center;
    font-size: 30px;
  }
  .subheader-content {
    text-align: justify;
    width: 75%;
  }
  .box-content h2,
  .body-box h1 {
    font-size: 20px;
  }
  .customer {
    display: flex;
    flex-direction: column;
    align-items: center;
  }

  .customer > img {
    margin-left: 0;
  }
  .box-content {
    display: flex;
    flex-direction: column;
    margin: 0%;
    width: auto;
  }
  .box-content-find {
    display: flex;
    flex-direction: column;
    padding: 0;
  }
  .box-content.home-video-container2 {
    margin: 0%;
    width: auto;
  }
  .box-test,
  .box-video {
    width: 87%;
  }
  .box-content > .box-test {
    margin: 2%;
    padding: 8%;
    width: auto;
  }
  .box-content > .box-test-content {
    width: 87%;
  }
  .box-content > .box-finder {
    margin: 2%;
    padding: 8%;
    border-radius: 10px;
    width: auto;
  }

  .box-content > .box-badges {
    width: 80%;
  }
  .box-content > .box-analysis {
    width: 80%;
  }

  .box-content-body {
    display: flex;
    flex-direction: column;
    padding-left: 0;
  }
  .box-video-content,
  .box-video-content-company {
    width: auto;
    margin: 2%;
    flex-direction: column;
  }
  .home-video-container2 .box-video-content {
    margin: 2%;
  }
  .box-video {
    width: 100%;
    display: flex;
    flex-direction: column;
  }

  .paragraph p,
  .para p {
    font-size: 25px;
    color: white;
    padding-left: 0;
  }
  .paragraph {
    padding: 5% 0% 0% 0%;
  }

  .sub-video {
    padding-inline-start: 0;
  }

  .box-content-analysis {
    width: 80%;
    padding: 5% 10% 0 15%;
  }

  .body-content {
    display: flex;
    flex-direction: column;
  }

  .box-content-page {
    display: flex;
    flex-direction: column-reverse;
    padding-left: 15%;
  }

  .box-content-finder {
    padding: 0 10% 0 20%;
    width: 80%;
    line-height: 30px;
    display: flex;
  }
  .slideshow-container {
    width: 70%;
  }
  .feedback {
    touch-action: cross-slide-x;
  }
  .box-content-finder h2 {
    padding-left: 35%;
    font-size: 50px;
  }
  .box-content-page .box-content-finder h2 {
    width: 80%;
    padding-left: 15%;
    letter-spacing: 0.1px;
    line-height: 20px;
  }
  .box-content p {
    padding-left: 0%;
  }
  .slider {
    padding: 50px 0 10% 0;
  }
  .slide {
    width: auto;
  }
  .quote,
  .invert {
    font-size: 3rem;
  }
  .image-slider p {
    width: 90%;
    font-size: 1rem;
  }

  /* index page ad video */
  .ad-video {
    width: 100%;
  }

  /* index page ad video container */
  #video-container,
  #mission-video-container,
  #student-video-container,
  #company-video-container {
    height: 70vh;
  }
}
@media only screen and (min-width: 641px) and (max-width: 768px) {
  .box-video-content,
  .box-video-content-company {
    flex-direction: column;
    width: 100%;
  }

  .para p,
  .paragraph p {
    font-size: 3.8vw;
    text-align: center;
  }
  .box-content p {
    padding-left: 0%;
  }
}
@media only screen and (min-width: 768px) and (max-width: 1024px) {
  .para p,
  .paragraph p {
    font-size: 3.8vw;
    text-align: center;
  }
  .header {
    text-align: center;
  }
  .subheader-content {
    text-align: justify;
  }
  .box-content-finder h2 {
    width: auto;
    height: 100px;
  }
  .box-video-content {
    display: flex;
    flex-direction: column;
  }
  .box-video-content,
  .box-video-content-company {
    flex-direction: column;
    width: 100%;
  }
  .box-content p {
    padding-left: 0%;
  }
  .box-content,
  .box-content.home-video-container2 {
    margin: 5%;
    width: auto;
  }
  .home-video-container2 .box-video-content,
  .box-video-content-company {
    margin-right: 0;
  }
  .box-content > .box-finder,
  .box-content > .box-test {
    width: 33%;
  }
}
</style>
