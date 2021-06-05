<template>
  <div class="wrapper">
    <div class="flex-row-center-space-even page-info">
      <div class="flex-col-center">
        <h2 class="info-header">Your Personal Mentor</h2>
        <p class="p-text text-center mt-10">
          An initiative by working professionals, to give back to students and
          share their knowledge to help them in career
        </p>
        <div class="button-align">
          <a
            href="https://forms.zohopublic.com/spotknack/form/Mission2021Registration/formperma/6HLkFAHXn-sAPii62-6vLCNSmx8Ys47CrrpEVJzgLSQ"
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
        src="https://spotknackcompanywebsite.s3.us-east-2.amazonaws.com/photos/mentor.PNG"
        width="100%"
        height="100%"
        alt="skillanalysis"
      />
    </div>
    <!-- You Are In Right Hands -->
    <div class="flex-row-center-space-even page-info">
      <div class="flex-col-center">
        <h2 class="info-header">You Are In Right Hands</h2>
        <p class="p-text text-center mt-10">
          You will have to switch from conventional ways of preparing for
          placement to become eligible to sit for placements. When it’s not
          going to conventional, why the same term placement preparation, lets
          the change call sign as preparing for Career.
        </p>
      </div>

      <img
        class="mentoring-images"
        src="https://spotknackcompanywebsite.s3.us-east-2.amazonaws.com/icons/mock.svg"
        width="100%"
        height="100%"
        alt="skillanalysis"
      />
    </div>
    <!-- Let’s Change -->
    <div class="flex-row-center-space-even page-info">
      <div class="flex-col-center">
        <h2 class="info-header">Let’s Change</h2>
        <p class="p-text text-center mt-10">
          The usual certification or training is just passive learning and
          working on projects. And watching videos of YouTube channels or
          certification may not complete your learning. You need something that
          gives you the feel of being professional.
        </p>
      </div>

      <img
        class="mentoring-images"
        src="https://spotknackcompanywebsite.s3.us-east-2.amazonaws.com/photos/change.PNG"
        width="100%"
        height="100%"
        alt="skillanalysis"
      />
    </div>

    <!-- And Evolve  -->
    <div class="flex-row-center-space-even page-info">
      <div class="flex-col-center">
        <h2 class="info-header">And Evolve</h2>
        <p class="p-text text-center mt-10">
          Let’s not spend our whole college to become eligible for placement or
          equip eligibility skills. Move on to unconventional ways of preparing,
          equipping yourself with employability skills that will make you be
          Skilful and sellable talent in the Job Market.
        </p>
      </div>

      <img
        class="mentoring-images"
        src="https://spotknackcompanywebsite.s3.us-east-2.amazonaws.com/photos/grow.PNG"
        width="100%"
        height="100%"
        alt="skillanalysis"
      />
    </div>
    <!-- Expectation from the company -->
    <div class="program-description">
      <h2 class="info-header">What We Expect From You,</h2>
      <ul class="program-list mt-15">
        <li>commitment</li>
        <li>Exploit our knowledge</li>
      </ul>
    </div>

    <!-- take away from us-->
    <div class="program-description">
      <h2 class="info-header">What you can take away from us,</h2>
      <ul class="program-list mt-15">
        <li>
          Overview of Different Job opportunities, while in college you are
          shown only narrowed down programming job.
        </li>
        <li>
          Guidelines or Ideas that will make you unique in the crowd, you have
          chosen the program, so you step ahead to be unique among the crowd.
        </li>
        <li>
          Reference for Jobs or Internships when you are a good performer after
          program completion.
        </li>
        <li>
          Project Ideas For College projects, which would increase your selling
          point in campus interview.
        </li>
        <li>Trends in the Companies Hiring Strategies.</li>
        <li>What would companies expect in a Resume and Interviews.</li>
        <li>Do’s and Don’ts while preparing the job.</li>
        <li>
          Say Goodbye to boring regular resume, while you’re Portfolio Will be
          ready to speak on behalf of you.
        </li>
        <li>
          While the majority of the crowd would have mentioned Database or Data
          Structures as their Area of Interest, choose your interest which you
          might have explored or found Interesting in the program.
        </li>
      </ul>
    </div>
    <!-- take away from You,-->
    <div class="program-description">
      <h2 class="info-header">What We Expect From You,</h2>
      <ul class="program-list mt-15">
        <li>
          I am not good in Aptitude and What if I don’t clear the aptitude round
        </li>
        <li>
          What if my scores are less and have not met the eligibility criteria
        </li>
        <li>
          Please make mistakes, if not you are not breaking things or learning
        </li>
        <li>
          Not the complete fear, sometimes fear is the one that will keep in
          track and kill building overconfidence in you, so we leave little fear
          in you, to keep in track.
        </li>
      </ul>
    </div>

    <!-- Our Goal -->
    <div class="program-description">
      <h2 class="info-header">Our Goal Is To,</h2>
      <ul class="program-list mt-15">
        <li>
          Make you earn money while studying in college, after completing the
          program
        </li>
        <li>
          Onboard you into the spotknack talent community, for a future job or
          Internship opportunities
        </li>
        <li>
          Make you self-reliant to find a job, irrespective of the job market
          situation
        </li>
        <li>
          Boost your confidence and give you a clarity of your career scope
        </li>
      </ul>
    </div>
    <!-- Mentoring program list with carousel design -->
    <div style="margin: auto">
      <h2 class="sub-header-H2">Mentoring For</h2>
      <p class="sm-font text-center">(Click On the Icons For Details)</p>
      <div class="flex-row-center-space-even carousel-container">
        <!-- Left arrow  -->
        <div
          id="previous-mentor"
          class="arrow-button"
          :class="[isLeftScrollDisable ? 'disabled' : '']"
          @click="scrollLeft"
        >
          &#x0003C;
        </div>
        <!-- Programs list Carousel -->
        <div class="mentor-container flex-div">
          <div
            class="flex-row-start carousel"
            :style="{ marginLeft: -(200 * marginLeftValue) + 'px' }"
          >
            <div
              v-for="(item, index) in items"
              :key="index"
              class="flex-col-center mentoring-career"
            >
              <a href="frontend_developer.html">
                <img :src="item.src" width="70" alt="" />
              </a>
              <p class="text">{{ item.name }}</p>
            </div>
          </div>
        </div>
        <!-- right arrow  -->
        <div
          id="next-mentor"
          class="arrow-button"
          :class="[isRightScrollDisable ? 'disabled' : '']"
          @click="scrollRight"
        >
          &#x0003E;
        </div>
      </div>
    </div>
  </div>
</template>

<script>
/* eslint no-console: ["error", { allow: ["warn", "log"] }] */

export default {
  data() {
    return {
      marginLeftValue: 0,
      items: [
        {
          name: 'Front End Developer',
          src: 'https://spotknackcompanywebsite.s3.us-east-2.amazonaws.com/icons/web+designer.png',
        },
        {
          name: 'App Developer',
          src: 'https://spotknackcompanywebsite.s3.us-east-2.amazonaws.com/icons/graphic-designer.png',
        },
        {
          name: 'Graphic Designer',
          src: 'https://spotknackcompanywebsite.s3.us-east-2.amazonaws.com/icons/graphic-designer.png',
        },
        {
          name: 'Content Writer',
          src: 'https://spotknackcompanywebsite.s3.us-east-2.amazonaws.com/icons/content.png',
        },
        {
          name: 'Front End Developer',
          src: 'https://spotknackcompanywebsite.s3.us-east-2.amazonaws.com/icons/web+designer.png',
        },
        {
          name: 'App Developer',
          src: 'https://spotknackcompanywebsite.s3.us-east-2.amazonaws.com/icons/graphic-designer.png',
        },
        {
          name: 'Graphic Designer',
          src: 'https://spotknackcompanywebsite.s3.us-east-2.amazonaws.com/icons/graphic-designer.png',
        },
        {
          name: 'Content Writer',
          src: 'https://spotknackcompanywebsite.s3.us-east-2.amazonaws.com/icons/content.png',
        },
      ],
      activeItem: 0, // track currently active item
      numOfItemToShow: 3, // No of items to be visible
    }
  },

  computed: {
    // disable left side scroll carousel functionality
    isLeftScrollDisable() {
      if (this.activeItem === 0) return true
      return false
    },
    // disable right side scroll carousel functionality
    isRightScrollDisable() {
      if (this.activeItem === this.items.length - this.numOfItemToShow)
        return true
      return false
    },
  },
  mounted() {
    // Check the useragent is mobile or not
    const isMobileDevice = /Mobi/i.test(window.navigator.userAgent)
    if (isMobileDevice) this.numOfItemToShow = 1
  },

  methods: {
    scrollRight() {
      this.activeItem += 1
      this.marginLeftValue += 1
    },
    scrollLeft() {
      this.activeItem += -1
      this.marginLeftValue += -1
    },
  },
}
</script>
<style scoped>
.disabled {
  opacity: 0.5;
  pointer-events: none;
  visibility: hidden;
}
.wrapper {
  margin: 7.6% 5%;
}
.program-description {
  margin-top: 70px;
}

.page-info .flex-col-center {
  margin-right: 5%;
  width: 60%;
}
.flex-row-center-space-even {
  margin-bottom: 10%;
}
.flex-row-center-space-even:nth-of-type(2n) {
  flex-direction: row-reverse;
}
.flex-row-center-space-even:nth-of-type(2n) > .flex-col-center {
  margin-left: 5%;
  margin-right: 0;
}
.program-list {
  list-style: url('~assets/images/green-circle.svg');
  margin-left: 6.7%;
}
.program-list li {
  margin-bottom: 10px !important;
}
.mentoring-career {
  min-width: 200px;
  cursor: pointer;
}
.carousel {
  transition: 500ms;
}
.carousel-container {
  width: 60%;
  margin: auto;
  overflow: hidden;
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
.arrow-button {
  font-size: 30px;
  cursor: pointer;
  z-index: 10;
}
.mentoring-career,
.arrow-button {
  user-select: none;
  -moz-user-select: none;
  -webkit-user-select: none;
  -ms-user-select: none;
}
.arrow-button:focus {
  fill: none;
}
.arrow-button:hover,
.mentoring-career:hover {
  opacity: 0.7;
}

/* Hide scrollbar for IE, Edge and Firefox */
.mentor-container {
  -ms-overflow-style: none; /* IE and Edge */
  scrollbar-width: none; /* Firefox */
  width: 600px;
  overflow: hidden;
}

/* Hide scrollbar for Chrome, Safari and Opera */
.mentor-container::-webkit-scrollbar {
  display: none;
}
@media only screen and (max-width: 1200px) {
  .carousel-container {
    width: auto;
  }
}
@media only screen and (min-width: 320px) and (max-width: 640px) {
  .flex-row-center-space-even,
  .flex-row-center-space-even:nth-of-type(2n) {
    flex-direction: column-reverse;
  }

  .page-info .flex-col-center {
    width: 90% !important;
    margin: auto;
  }
  .carousel-container {
    flex-direction: row !important;
  }

  /* .carousel {
    overflow-x: scroll;
  } */
  .mentor-container {
    width: 200px !important;
    overflow: hidden;
  }
}
</style>
