<template>
  <div class="wrapper">
    <img
      src="~assets/images/Spotknacklogo.svg"
      alt="Spotknack"
      class="Group-Copy logo-company-header"
    />
    <h1 class="info-header">TERMS OF SERVICE AGREEMENT</h1>

    <ol class="guideline-item-wrapper" type="I">
      <h6 class="header-description-content mt-15">
        LAST REVISION: [30.07.2019]
      </h6>
      <div class="mt-15 guide-line-content">
        <p class="mt-10">
          PLEASE READ THIS TERM OF SERVICE AGREEMENT CAREFULLY. BY USING THIS
          WEBSITE OR ORDERING PRODUCTS FROM THIS WEBSITE YOU AGREE TO BE BOUND
          BY ALL OF THE TERMS AND CONDITIONS OF THIS AGREEMENT.
        </p>
      </div>
      <li v-for="item in items" :key="item.id" class="mt-15 guideline-item">
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
      </li>
    </ol>
  </div>
</template>
<script>
export default {
  data() {
    return {
      items: [
        {
          id: 1,
          header: 'PRODUCTS',
          subHeaderContents: [
            'Terms of Offer. This Website offers for sale certain test and other offers. By placing an order for test and other offers through this Website, you agree to the terms set forth in this Agreement.',
            ' Solicitation Unless you notify our third party call center reps or direct Spotknack sales reps, while they are calling you, of your desire to opt out from further direct company communications and solicitations, you are agreeing to continue to receive further emails and call solicitations Spotknack Private Limited and its designated in house or third party call team(s).',
            'Out Procedure: We provide 3 easy ways to opt out of from future solicitations. 1. You may  use the opt out link found in any email solicitation that you may receive. 2. You may also choose to opt out, via sending your email address to: teamSpotknack@gmail.com Proprietary Rights. Spotknack has proprietary rights and trade secrets in the Products. You may not copy, reproduce, resell or redistribute any Product or service offered and/or  distributed by Spotknack.  Spotknack also has rights to all trademarks and trade dress and specific layouts of this webpage, including  calls to action, text placement, images and other information.',
            'Sales Tax. If you purchase any Products, you will be responsible for paying any applicable sales tax.',
          ],
        },
        {
          id: 2,
          header: 'WEBSITE',
          subHeaderContents: [
            'Content; Intellectual Property; Third Party Links. In addition to making Products available, this Website also offers information and marketing materials. This Website also offers information, both directly and through indirect links to third-party websites, about promo codes and links to share data with companies. Spotknack Private Limited does not always createthe information offered on this Website; instead the information is often gathered from other sources. To the extent that SpotknackPrivate Limited does create the content on this Website, such content is protected by intellectual property laws of the India, foreign nations, and international bodies. Unauthorized use of the material may violate  copyright, trademark, and/orother laws. You acknowledge that your use of the content on this Website is for personal, noncommercial use.  Any links to third-party websites are provided solely as a convenience to you. Spotknack does not endorse the contents on any such  third-party websites. Spotknack is not responsible for the content of or any damage that may result from your access to or reliance on these third-party websites. If you link to third-party websites, you do so at your own risk. Use of Website;',
            ' Spotknack is not responsible for any damages resulting from use of this website by anyone. You will not use the Website for illegal purposes. You will (1) abide by all applicable local, state, national, and international laws and regulations in your use of the Website (including laws regarding intellectual property), (2) not interfere with or disrupt the useand enjoyment of the Website by other users, (3) not resell material on the Website, (4) not engage,directly or indirectly, in transmissionof "spam", chain letters, junk mail or any other type of unsolicited communication, and (5) not defame,harass, abuse, or disrupt other users of the Website',
            'License. By using this Website, you are granted a limited, non-exclusive, nontransferable right to use thecontent and materials on the Website in connection with your normal, noncommercial, use of the Website. You may not copy, reproduce, transmit, distribute,or create derivative works of such content or information without express written authorization from Spotknack or the applicable third party (if third party content is at issue).',
            '  Posting. By posting, storing, or transmitting any content on the Website, you hereby grant Spotknack aperpetual, worldwide, non-exclusive, royalty-free, assignable, right and license to use, copy, display,perform, create derivative works from, distribute  have distributed, transmit and assign such content in any form, in all media now known or here in aftercreated, anywhere in the world. Spotknack Private Limited does not have the ability to control the nature ofthe user-generated content offered through the Website. You are solely responsible for your interactions with other users of the Website and any content you post. Spotknack is not liable for any damage or harm resulting from any posts by or interactions between users. Spotknack reserves the right, but has no obligation, to monitor interactions between and among users of the Website and to remove any content.',
          ],
        },
        {
          id: 3,
          header: ' DISCLAIMER OF WARRANTIES',
          subHeaderContents: [
            '  Your use of this website and/or products are at your sole risk. the website and products are offered on an "as is" and "as available" basis. spotknack expressly disclaims all warranties of any kind, whether expressor implied, including, but not limited to, implied warranties of merchantability, fitness for a particular purpose and noninfringement with respect to the products or website content, or any reliance upon or use of the website content or products.("products" include trial products.)',
            'Without limiting the generality of the foregoing, spotknack private limited makes no warranty:',
            'That the information provided on this website is accurate, reliable, complete, or timely.',
            'That the links to third-party websites are to information that is accurate, reliable, complete, or timely.',
            'No advice or information, whether oral or written, obtained by you from this website will create any warranty not expressly stated herein.',
            'As to the results that may be obtained from the use of the products or that defects in products will be  corrected.',
            'Regarding any products purchased or obtained through the website.',
            'Some jurisdictions do not allow the exclusion of certain warranties, so some of the above exclusions may not apply to you.',
          ],
        },
        {
          id: 4,
          header: 'LIMITATION OF LIABILITY',
          subHeaderContents: [
            ' Spotknack entire liability, and your exclusive remedy, in law, in equity, or othwerwise, with respect to the website content and products and/or for any breach of this agreement is solely limited to the amount you  paid, less shipping and handling, for  products purchased via website.',
            'Spotknack will not be liable for any direct, indirect, incidental, special or consequential damages in connection with this agreement or the products in any manner, including liabilities resulting from (1) the use or the inability to use the website content or products; (2) the cost of procuring substitute products or content; (3) any products purchased or obtained or transactions entered into through the website; or (4) any lost profits you allege.',
            ' Some jurisdictions do not allow the limitation or exclusion of liability for incidental or consequential damages so some of the above limitations may not apply to you.',
          ],
        },
        {
          id: 5,
          header: ' INDEMNIFICATION',

          subHeaderContents: [
            "You will release, indemnify, defend and hold harmless Spotknack, and any of its contractors, agents, employees, officers, directors, shareholders, affiliates and assigns from all liabilities, claims, damages, costs and expenses, including reasonable attorneys'      fees and expenses, of third parties relating to or arising out of (1) this Agreement or the breach of your     warranties, representations and obligations under this Agreement; (2) the Website content or your use of the Website content; (3) the Products or your use of the Products (including Trial Products); (4) any intellectual property or other proprietary right of any person or entity; (5) your violation of any provision of this Agreement; or (6) any  information or data you supplied  to Spotknack. When Spotknack is threatened with suit or sued by a third party, Spotknack may seek written  assurances from you concerning your promise to indemnify Spotknack Private Limited; your failure to provide such assurances may be considered by Spotknack to be a material breach of this Agreement. Spotknack Private Limited will have the toparticipate in any defense by you of a third-party claim related to your use of any of the Website content or Products, with counsel of  Spotknack choice at its expense. Spotknack will reasonably cooperate in any defense by you of a third-party claim at your request and expense. You will have sole responsibility to defend Spotknack against any claim,  but you must receive Spotknack prior written consent regarding any related settlement. The terms of this provision will survive any termination or cancellation of this Agreement or your use of the Website or Products. ",
          ],
        },

        {
          id: 6,
          header: 'PRIVACY',
          subHeaderContents: [
            'Spotknack believes strongly in protecting user privacy and providing you with notice of use of data. Please refer to Spotknack privacy policy, incorporated by reference herein, that is posted on the Website. ',
          ],
        },

        {
          id: 7,
          header: 'AGREEMENT TO BE BOUNDS',
          subHeaderContents: [
            'By using this Website or ordering Tests/Products or other offers, you acknowledge that you have read and agree to be bound by this Agreement and all terms and conditions on this Website.',
          ],
        },

        {
          id: 8,
          header: 'ACCOUNT TERMINATION CONDITIONS',
          subHeaderContents: [
            '  The account of the user will be terminated with or without prior notice when these following usage policy are violated.',
            '1. Posting inappropriate contents in the discussion forum and misusing the platform.',
            '2. Using the data of the portal for any commercial or promotion without our acknowledge.',
            '3. Users who are been black listed by the company Spotknack on many conditions and violating the company policies.',
            '4. If all the  details(Certificates, Workshop , Project , Internship, Roll Number and all other personal details) provided are found to be fake.',
          ],
        },

        {
          id: 9,
          header: 'GENERAL',
          subHeaderContents: [
            ' Force Majeure. Spotknack will not be deemed in default hereunder or held responsible for any cessation,interruption or delay in the performance of its obligations hereunder due to earthquake, flood, fire, storm,natural disaster, act of God, war, terrorism,armed conflict, labor strike, lockout, or boycott. Cessation of Operation. Spotknack may at any time, in its sole discretion and without advance notice to you, cease operation of the Website and distribution of the Products.',
            'Entire Agreement. This Agreement comprises the entire agreement between you and Spotknack and supersedes any prior agreements pertaining to the subject matter contained herein.',
            'Effect of Waiver. The failure of Spotknack to exercise or enforce any right or provision of this Agreement will not constitute a waiver of such right or provision. If any provision of this Agreement is found by a court of competent jurisdiction to be invalid, the parties nevertheless agree that the court should endeavor to give effect to the parties "intentions as reflected in the provision, and the other provisions of this Agreement remain in full force and effect."',
            'Governing Law; This Website originates from the Coimbatore ,Tamil Nadu. This Agreement will be governed by the laws of the State without regard to its conflict of law principles to the contrary. Neither you nor Spotknack will commence or prosecute any suit, proceeding or claim to enforce the provisions of this Agreement, to recover damages for breach of or default of this Agreement, or otherwise arising under or by reason of this Agreement, other than in courts located in State of TamilNadu. By using this Website or ordering Products, you consent to the jurisdiction and venue of such courts in connection with any action, suit, proceeding or claim arising under or by reason of this Agreement Youhereby waive any right to trial by jury arising out of this Agreement and any related documents.',
            ' Statute of Limitation. You agree that regardless of any statute or law to the contrary, any claim or cause of action arising out of or related to use of the Website or Products or this Agreement must be filed within one (1) year after such claim or cause of action arose or be forever barred.',
            'Waiver of Class Action Rights.BY ENTERING INTO THIS AGREEMENT, YOU HEREBY IRREVOCABLY WAIVE ANY RIGHT YOU MAY  HAVE TO JOIN CLAIMS WITH THOSE OF OTHER IN THE FORM OF A CLASS ACTION OR SIMILAR PROCEDURAL DEVICE. ANY CLAIMS ARISING OUT OF, RELATING TO, OR CONNECTION WITH THIS AGREEMENT MUST BE ASSERTED INDIVIDUALLY.',
            'Termination. Spotknack reserves the right to terminate your access to the Website if it reasonably believes, in its sole discretion, that you have breached any of the terms and conditions of this Agreement. Following termination, you will not be permitted to use the Website and Spotknack may, in its sole discretion and without advance notice to you, cancel any outstanding orders for Products. If your access to the Website is terminated, Spotknack reserves the right to exercise whatever means it deems necessary to prevent unauthorized access of the Website. This Agreement will survive  indefinitely unless and until Spotknack chooses, in its sole discretion and without advance to you, to terminate it.',
            '  Domestic Use. Spotknack makes no representation that the Website or Products are appropriate or available for use in locations outside India. Users who access the Website from outside India do so at their own risk and initiative and must bear all responsibility for compliance with any applicable local laws.',
            ' Assignment. You may not assign your rights and obligations under this Agreement to anyone. Spotknack may assign its rights and obligations under this Agreement in its sole discretion and without advance notice to you.',
            'BY USING THIS WEBSITE OR ORDERING PRODUCTS FROM THIS WEBSITE YOU AGREE TO BE BOUND BY ALL OF THE TERMS ANDCONDITIONS OF THIS AGREEMENT.',
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
