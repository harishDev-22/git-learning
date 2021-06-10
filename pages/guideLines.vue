<template>
  <div class="wrapper">
    <img
      src="~assets/images/Spotknacklogo.svg"
      alt="Spotknack"
      class="Group-Copy logo-company-header"
    />
    <h1 class="info-header">Guidelines</h1>
    <p class="p-text text-center mt-22">
      Our code of Contact and your pledge to adhere to the spotknack community
      guidelines.
    </p>
    <div class="guideline-item-wrapper">
      <div v-for="item in items" :key="item.id" class="mt-15 guideline-item">
        <h6 class="header-description-content">
          <span class="guide-item-index playfair-font"> {{ item.id }}.</span>
          {{ item.header }}
        </h6>
        <div v-if="item.subHeader" class="mt-15 guide-line-content">
          <p>
            {{ item.subHeader }}
          </p>
          <ol>
            <li
              v-for="(content, index) in item.subHeaderContents"
              :key="index"
              class="mt-15"
            >
              {{ content }}
            </li>
          </ol>
          <p v-if="item.subHeader2" class="mt-15">
            {{ item.subHeader2 }}
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
          id: 1,
          header: 'I will upload only work that I’ve created',
          subHeader:
            ' Share your own work on Spotknack (Projects,Contents,Certifications).',
          subHeader2: '',
          subHeaderContents: [
            'Don’t post others’ work.',
            'Don’t take credit for others’ work.',
            'Don’t post copyrighted or trademarked content.',
          ],
        },
        {
          id: 2,
          header: 'I won’t post inappropriate content ',
          subHeader:
            'Spotknack aspires to be a welcoming and inclusive community. Please don’t post content that is:',
          subHeader2:
            'If you post inappropriate content, it may be removed by Dribbble per our Terms of Service. Dribbble has final say over whether content is appropriate. If you repost content that’s been removed or continue to post content that violates these guidelines your account may be suspended or removed.',
          subHeaderContents: [
            'Illegal',
            'Mature in content, or gratuitously or overly sexual.',
            'Racist, sexist, or otherwise offensive words.',
            'Inflammatory (e.g. name-calling, preaching, ranting, stirring up controversy, or venting frustrations)',
          ],
        },
        {
          id: 3,
          header: 'I won’t spam other Spotknack Members',
          subHeader:
            ' Spotknack provides certain features that allow users to interact with one-another, including messages. Please don’t use these tools indiscriminately to spam or send unsolicited messages to other members. If you’re caught spamming other Spotknack users, your account may be suspended or removed and and it may sometimes lead to legal actions. Don’t do the following,',
          subHeader2: '',
          subHeaderContents: [
            'Leaving many comments that are short on substance to draw attention to your account',
            'Misusing the site features or functionality in a way that isn’t in line with their core purpose forpersonal gain.',
          ],
        },
        {
          id: 4,
          header: 'Multiple Accounts',
          subHeader:
            ' Don’t create multiple accounts if your scores in the verified or first account is poor. Try to improve to performance by necessary steps.',
          subHeader2: '',
          subHeaderContents: [],
        },
        {
          id: 5,
          header: ' Being Genuine to know your Strengths',
          subHeader:
            'Never involve in malpractices to improve your test scores. Don’t do the following',
          subHeader2:
            'If you notice any Spotknack user involving in malpractice to improve their scores or their ranking, you can mail us to support@spotknack.com along with proof. Team would take necessary steps if proven.',
          subHeaderContents: [
            ' Referring Google and other online websites to find clues or answers for the questions.',
            'Trying to extract the questions.',
            'Don’t attempt tests or contests from your friends account.',
          ],
        },
      ],
    }
  },
}
</script>

<style scoped>
.guideline-item-wrapper {
  margin: 43px 22.4% 43px 8.1%;
}
.wrapper {
  margin: auto;
  margin-bottom: 60px;
}
.guideline-item:nth-of-type(1) {
  margin-top: 22px !important;
}
.guide-line-content > * {
  opacity: 0.7;
  font-size: 12px;
  font-weight: normal;
  font-stretch: normal;
  font-style: normal;
  line-height: 1.67;
  letter-spacing: 0.6px;
  color: #000;
}

.guide-line-content li,
ol {
  padding: 0 !important;
  margin: 0 !important;
}
.guide-line-content ol {
  padding-left: 15px !important;
  margin-left: 0 !important;
}
.guide-item-index {
  font-size: 14px;
  font-weight: bold;
  font-stretch: normal;
  font-style: normal;
  line-height: normal;
  letter-spacing: 2px;
  color: #000;
  padding: 7px;
  background-color: #c9fd6a;
  border-radius: 50%;
  margin-left: -5px !important;
  text-align: center;
  margin-right: 10px !important;
}
@media only screen and (max-width: 640px) {
  .wrapper {
    width: 80%;
    margin: 43px auto;
  }
  .guideline-item-wrapper {
    width: auto;
    margin: auto;
  }
  .guide-item-index {
    font-size: 12px;
    padding: 5px;
  }
}
</style>
