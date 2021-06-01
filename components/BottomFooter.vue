<template>
  <footer>
    <div class="footer">
      <div class="spot">
        <img src="~assets/images/Logofooter.svg" width="200" alt="logo" />
      </div>
      <div class="footer-line">
        <div class="footer-content">
          <div class="foot">
            <p>Menu</p>
            <NuxtLink to="/"> Home </NuxtLink>
            <NuxtLink to="/about">About </NuxtLink>
            <NuxtLink
              v-b-tooltip.hover
              title=" Mock Interview"
              to="/mockInterview"
            >
              Mock Interview
            </NuxtLink>
            <NuxtLink to="/mockInterview"> Student Programs </NuxtLink>

            <a
              href="https://recruit.zohopublic.com/recruit/Portal.na?iframe=false&digest=.WsqhQLLOxoxOoGMDi%40yUnGAUnkE7bVo.a85bxdBEmQ-"
              target="blank"
            >
              Career
            </a>
            <a href="http://bit.ly/spotknack_career_document" target="blank">
              Contribute
            </a>
          </div>
          <div class="foot">
            <p>Resources</p>
            <a href="https://blog.spotknack.com" target="blank"> Blog </a>
            <NuxtLink to="/">FAQ </NuxtLink>
            <NuxtLink to="/">Guidelines </NuxtLink>
            <NuxtLink to="/">Terms and Conditions </NuxtLink>
            <NuxtLink to="/">Privacy Policy </NuxtLink>
          </div>
          <div class="foot">
            <p>Company</p>
            <NuxtLink to="/">Mentees </NuxtLink>
            <a href="https://spotknack.com/views/mission2021/">
              Mission 2021
            </a>
            <NuxtLink to="/">Campus Ambassadors </NuxtLink>
            <NuxtLink to="/">Spotknack for Startups </NuxtLink>
            <NuxtLink to="/">Spotknack for Educators </NuxtLink>
            <NuxtLink to="/">Donate </NuxtLink>
          </div>

          <div class="foot">
            <p>Featured On</p>
            <a
              href="https://www.edexlive.com/happening/2021/mar/17/heres-how-spotknack-is-securing-employment-opportunities-for-the-average-student-19088.html"
            >
              Indian Express - Edex
            </a>
          </div>
        </div>
        <!--Google map integration -->

        <div class="map">
          <p>Come meet us here !</p>
          <iframe
            src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3915.4328324686107!2d76.98652631480348!3d11.081083792115216!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x0%3A0x5e517072b067391b!2siBevy+Forte!5e0!3m2!1sen!2sin!4v1562062625961!5m2!1sen!2sin"
            frameborder="0"
            style="border: 0"
            allowfullscreen
          ></iframe>
        </div>
      </div>
      <!--social media icons -->
      <div class="social-icons">
        <div class="icons">
          <p>Social</p>
          <a href="https://facebook.com/spotknack" target="blank"
            ><img src="~assets/images/facebook.png" width="30" alt="facebook"
          /></a>
          <a href="https://facebook.com/spotknack" target="blank"
            ><img src="~assets/images/linkedin.png" width="30" alt="facebook"
          /></a>
          <a href="https://facebook.com/spotknack" target="blank"
            ><img src="~assets/images/instagram.png" width="30" alt="facebook"
          /></a>

          <a href="https://linkedin.com/company/spotknack" target="blank"
            ><img src="~assets/images/twitter.png" width="30" alt="linkedin"
          /></a>
        </div>
      </div>
      <div class="copyright">
        <div class="text">
          <p>2021 &copy; Spotknack</p>
        </div>
      </div>
    </div>
  </footer>
</template>
<script>
export default {
  methods: {
    openHomepage() {
      this.$router.push('/')
    },
  },
}
</script>
<style scoped>
/*  footer */
.footer {
  width: 100%;
  background-color: #131415;
  height: auto;
  padding: 100px 0 20px 8.6%;
}
.footer-line {
  display: flex;
  flex-direction: row;
  width: 100%;
}

.foot {
  width: 100%;
  display: flex;
  flex-direction: column;
}
.foot a {
  text-decoration: none;
  color: white;
  line-height: 30px;
}
.foot li {
  list-style-type: none;
  font-size: 1rem;
}
.map {
  width: 26.3%;
  padding-right: 8.5%;
}
.map li {
  list-style-type: none;
}
.map iframe {
  border-radius: 20px;
  width: 100%;
  height: 60%;
}
.footer-content {
  width: 73.7%;
  display: flex;
  flex-direction: row;
}

/*  social icons in the footer */

.icons a {
  padding-right: 2%;
}
.copyright {
  padding-top: 1%;
}
.foot p,
.map p {
  color: white;
  opacity: 0.3;
  font-size: 1.25rem;
  margin-top: 20px;
}

.icons p {
  color: white;
  opacity: 0.3;
  font-size: 1.25rem;
}
.text p {
  color: white;
  opacity: 0.3;
  font-size: 1.0625rem;
}
.header {
  width: 100%;
  margin-top: 80px;
}
.foot a:hover,
.social-icons a:hover {
  opacity: 0.8;
}

@media only screen and (max-width: 768px) {
  .footer-line {
    display: flex;
    flex-direction: column;
    width: 100%;
  }

  .footer-content {
    display: flex;
    flex-direction: column;
  }

  .foot li {
    font-size: 1rem;
  }

  .map {
    width: 50%;
    margin: 0;
    padding-left: 0;
  }
  .social-icons {
    margin-top: 10px;
  }
  .copyright {
    margin-top: 20px;
  }
}
@media only screen and (max-width: 640px) {
  .footer-line {
    display: flex;
    flex-direction: column;
  }
  footer {
    height: 800px;
  }

  .foot {
    padding-right: 20%;
  }
  .foot li {
    font-size: 0.75rem;
  }

  .foot ul {
    width: 118%;
  }
  .footer-content {
    padding-left: 0;
    width: auto;
  }
  .map {
    width: 100%;
    margin: 0;
    padding-left: 0;
  }
  .journey {
    margin-top: 10%;
  }
}
@media only screen and (max-width: 991px) and (min-width: 769px) {
  .footer-line {
    display: flex;
    flex-direction: column;
    width: 100%;
  }
  .footer-content {
    width: 90%;
    padding-left: 0;
  }
  .map {
    width: 50%;
    margin: auto;
  }

  .foot {
    /* padding-right:10%; */
    width: 100%;
  }
  .foot li {
    font-size: 1.7vw;
  }

  .foot:not(p) {
    font-size: 0.75em;
  }

  /* .footer-content {
    padding-left: 0;
  } */
}
@media only screen and (min-width: 768px) and (max-width: 1024px) {
  .foot li {
    font-size: 0.7rem;
  }
  .foot > p,
  .map > p {
    font-size: 14px;
  }
}
</style>
