<template>
  <div class="wrapper">
    <img
      src="~assets/images/Spotknacklogo.svg"
      alt="Spotknack"
      class="Group-Copy logo-company-header"
    />
    <h1 class="info-header">Privacy Policy</h1>

    <div class="guideline-item-wrapper">
      <div v-for="item in items" :key="item.id" class="mt-15 guideline-item">
        <h6 class="header-description-content">
          {{ item.header }}
        </h6>
        <div class="mt-15 guide-line-content">
          <p
            v-for="(content, index) in item.subHeaderContents"
            :key="index"
            class="mt-10"
          >
            {{ content }}
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
          header: 'General',

          subHeaderContents: [
            'The url https://spotknack.com website, which provides the SERVICE.',
            'This page is used to inform website visitors regarding our policies with the collection, use, and disclosure of Personal Information if anyone decided to use our Service.',
            'If you choose to use our Service, then you agree to the collection and use of information in relation with this policy. The Personal Information that we collect are used for providing and improving the Service. We will not use or share your information  with anyone except as described in this Privacy Policy.',
            'The terms used in this Privacy Policy have the same meanings as in our Terms and Conditions, which is accessible at https://spotknack.com , unless otherwise defined in this Privacy Policy.',
          ],
        },
        {
          id: 2,
          header: 'Information Collection and Use ',
          subHeaderContents: [
            'For a better experience while using our Service, we may require you to provide us with certain personally identifiable information, including but not limited to your name, phone number, and postal address. The information that we collect will be used to contact or identify you.',
          ],
        },
        {
          id: 3,
          header: 'Log Data',
          subHeaderContents: [
            'We want to inform you that whenever you visit our Service, we collect information that your browser sends to us that is called Log Data. This Log Data may include information such as your computers Internet Protocol (IP) address, browser version, pages of our Service that you visit, the time and date of your visit, the time spent on those pages, and other statistics.',
          ],
        },
        {
          id: 4,
          header: 'Cookies',
          subHeaderContents: [
            'Cookies are files with small amount of data that is commonly used an anonymous unique identifier. These are sent to your browser from the website that you visit and are stored on your computers hard drive.',
            'Our website uses these cookies to collection information and to improve our Service. You have the option to either accept or refuse these cookies, and know when a cookie is being sent to your computer. If you choose to refuse our cookies, you may not be able to use some portions of our Service.',
          ],
        },
        {
          id: 5,
          header: ' Service Providers',

          subHeaderContents: [
            'We may employ third-party companies and individuals due to the following reasons:',
            'To facilitate our Service;',
            'To provide the Service on our behalf;',
            'To perform Service-related services; or',
            'To assist us in analyzing how our Service is used.',
            'We want to inform our Service users that these third parties(Companies) have access to your Personal Information only after prior approval from the us. The reason is to perform the tasks assigned to them on our behalf. However, they are obligated not to disclose or use the information for any other purpose.',
          ],
        },

        {
          id: 6,
          header: 'Security',
          subHeaderContents: [
            'We value your trust in providing us your Personal Information, thus we are striving to use commercially acceptable means of protecting it. But remember that no method of transmission over the internet, or method of electronic storage is 100% secure and reliable, and we cannot guarantee its absolute security.',
            'When companies subscirbe to our platform to view your skill data, we will be disclosing your Name,College Name and your skill details.But your contact number and email will not be disclosed to them unless you approve to share your contact details',
          ],
        },

        {
          id: 7,
          header: 'Links to Other Sites',
          subHeaderContents: [
            'Our Service may contain links to other sites. If you click on a third-party link, you will be directed to that site. Note that these external sites are not operated by us. Therefore, we strongly advise you to review the Privacy Policy of these websites. We have no control over, and assume no responsibility for the content, privacy policies, or  practices of any third-party sites or services.',
          ],
        },

        {
          id: 8,
          header: 'Childrens Privacy',
          subHeaderContents: [
            'Our Services do not address anyone under the age of 13. We do not knowingly collect personal identifiable information from children under 13. In the case we discover that a child under 13 has provided us with personal information, we immediately  delete this from our servers. If you are a parent or guardian and you are aware that your child has provided us with personal information, please contact us so that we will be able to do necessary actions.',
          ],
        },

        {
          id: 9,
          header: 'Collge Policy',
          subHeaderContents: [
            'To college subscribers, we do not take the responsibility of data originality that appear on your dashboard.We exactly produce data that our candidate provide and update in their portal.',
            '  And if you are not able to view or access the data of your students, please ask your students to check details he/she updated in their portal. We do not take the responsibility for it. The entire process is automated with provided data.',
          ],
        },

        {
          id: 10,
          header: 'Changes to This Privacy Policy',
          subHeaderContents: [
            'For a better experience while using our Service, we may require you to provide us with certain personally identifiable information, including but not limited to your name, phone number, and postal address. The information that we collect will be used to contact or identify you.',
          ],
        },
        {
          id: 11,
          header: 'Contact Us',
          subHeaderContents: [
            'If you have any questions or suggestions about our Privacy Policy, do not hesitate to contact us.',
          ],
        },
      ],
    }
  },
}
</script>

<style scoped>
.guideline-item-wrapper {
  margin: 43px 8.1%;
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

.guide-line-content p {
  margin-bottom: 0 !important;
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
}
</style>
