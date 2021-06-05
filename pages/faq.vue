<template>
  <div class="wrapper">
    <h3 class="sub-header-H3">Frequently Asked Questions</h3>
    <div v-for="item in items" :key="item.id" class="faq-container">
      <!-- v-b-toggle is a question reference  -->
      <!-- item.active data toggles the style between plus and minus icon -->
      <p
        v-b-toggle="item.id.toString()"
        class="m-1 playfair-font flex-row-center-space-bw"
        :class="{ activefaq: item.active }"
        @click="item.active = !item.active"
      >
        {{ item.question }} ?
        <span :class="[item.active ? 'activefaqIcon' : 'plus-icon']">
          <b class="plus-b" :class="{ activefaq: item.active }">
            {{ item.active ? '-' : '+' }}</b
          ></span
        >
      </p>
      <!-- Element to collapse -->
      <!-- b-collapse id is a answer reference  -->

      <b-collapse :id="item.id.toString()">
        <b-card class="faq-answer playfair-font">{{ item.answer }}</b-card>
      </b-collapse>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      // faq list items
      items: [
        {
          id: '1',
          active: false,
          question: 'What is a Scoreboard?',
          answer:
            'The maximum credit for a test is 6. Earn 18 credits to unlock a new badge. It is the place where you can find the scores for every test you have taken in every category.',
        },
        {
          id: '2',
          active: false,
          question: 'What is a Leaderboard',
          answer:
            'This menu will show your rank among the users of the forum respective to the tests.',
        },
        {
          id: '3',
          active: false,
          question:
            'Why should the user provide priority of interest in the profile Form',
          answer:
            'Based on the priority you choose, we at iBevy, will suggest you information and scope for development in the Newsfeed of the portal.',
        },

        {
          id: '4',
          active: false,
          question:
            'Why do we have to upload a photocopy of the college ID card',
          answer: 'We collect it to verify your identity.',
        },
        {
          id: '5',
          active: false,
          question: 'Is it possible to retake a test once it is submitted',
          answer: 'No, a test can be taken only once.',
        },
        {
          id: '7',
          active: false,
          question: 'Do I have to pay to use the platform',
          answer:
            'Majority of the features are made free for students to help reach everyone.',
        },
        {
          id: '8',
          active: false,
          question: 'How the skill finder works to connect with other friends',
          answer:
            'Once you search through the portal for a particular skill, you can find the list of students displayed. Once you click for a request to connect with them, your mail id will be shared with them to contact you.',
        },
        {
          id: '9',
          active: false,
          question:
            'Is it possible to change the Mail id and Name once updated?',
          answer:
            'No, you cannot change it. You may like to know that these basic details will be shared to potential companies looking for candidates like you. Changing the name and mail I’d lead tounwanted ambiguity. If you do not have access to the registered mail account, contact us through teamibevy@gmail.com.',
        },
        {
          id: '10',
          active: false,
          question: 'What is the use of Newsfeed',
          answer:
            'The newsfeed is the place where we will post News and Advertisements based on your Priority index given in the profile.',
        },
      ],
    }
  },
}
</script>
<style scoped>
.wrapper {
  width: 72.1%;
  margin: 43px 22.4% 43px 5.5%;
}
.sub-header-H3 {
  margin-top: 10%;
}
.collapse .card {
  border: none;
  border-top: 1px solid #3bd8d4;
  border-radius: 0;
}

.faq-container > p {
  border-top: 1px solid rgba(20, 20, 20, 0.2);
  padding: 10px;
  font-size: 16px;
  font-weight: normal;
  font-stretch: normal;
  font-style: normal;
  line-height: 1.75;
  letter-spacing: 0.6px;
  word-break: break-word;
}

/* Active element */
.activefaq {
  color: #3bd8d4 !important;
}

.plus-icon {
  float: right;
  min-width: 35px;
  height: 35px;
  border: solid 3px rgba(0, 0, 0, 0.5);
  text-align: center;
  border-radius: 50%;
  line-height: 1.75;
  font-size: 20px;
  position: relative;
}

/* Active icon with blue color */
.activefaqIcon {
  color: #3bd8d4 !important;
  border: solid 3px #3bd8d4 !important;
  float: right;
  min-width: 35px;
  height: 35px;
  text-align: center;
  border-radius: 50%;
  line-height: 1.75;
  font-size: 20px;
  position: relative;
}

/* icon text style */
.plus-b {
  position: relative;
  top: -2px;
  font-size: 24px;
  font-weight: bold;
  font-stretch: normal;
  font-style: normal;
  line-height: 1.17;
  letter-spacing: 0.6px;
  color: rgba(0, 0, 0, 0.5);
}

/* disable double icon */
.plus-icon,
.faq-container > p {
  user-select: none;
  -moz-user-select: none;
  -webkit-user-select: none;
  -ms-user-select: none;
}
.faq-answer {
  font-size: 12px;
  font-weight: normal;
  font-stretch: normal;
  font-style: normal;
  line-height: 2.33;
  letter-spacing: 0.6px;
  color: #000;
}
.faq-container:nth-of-type(1) > p {
  border: none;
}
.faq-container:nth-of-type(1) {
  margin-top: 43px;
}
.card-body {
  padding: 1.5rem;
}
.collapse .card :nth-child(1) {
  border-top: none;
}

@media only screen and (max-width: 640px) {
  .wrapper {
    width: 90%;
    margin: 43px auto;
  }
}
</style>
