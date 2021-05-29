<template>
  <footer>
    <div class="footer">
      <div class="spot">
        <img src="~assets/images/Logofooter.svg" width="200" alt="logo" />
      </div>
      <div class="footer-line">
        <div class="footer-content">
          <div class="foot">
            <ul>
              <p>Menu</p>
              <a href="views/about.html">
                <li>About</li>
              </a>
              <a href="index.html">
                <li>Home</li>
              </a>
              <a href="views/mockinterview.html" target="blank">
                <li>Mock Interview</li>
              </a>
              <a href="views/student_mentoring.html" target="blank">
                <li>Student Programs</li>
              </a>
              <a
                href="https://recruit.zohopublic.com/recruit/Portal.na?iframe=false&digest=.WsqhQLLOxoxOoGMDi%40yUnGAUnkE7bVo.a85bxdBEmQ-"
                target="blank"
              >
                <li>Career</li>
              </a>
              <a href="http://bit.ly/spotknack_career_document" target="blank">
                <li>Contribute</li>
              </a>
            </ul>
          </div>
          <div class="foot">
            <ul>
              <p>Resources</p>
              <a href="https://blog.spotknack.com" target="blank">
                <li>Blog</li>
              </a>
              <a href="views/faq.html" target="">
                <li>FAQ</li>
              </a>

              <a href="views/guidelines.html" target="blank">
                <li>Guidelines</li>
              </a>
              <a href="views/terms and conditions.html" target="blank">
                <li>Terms and Conditions</li>
              </a>
              <a href="views/privacypolicy.html" target="blank">
                <li>Privacy Policy</li>
              </a>
            </ul>
          </div>

          <div class="foot">
            <ul>
              <p>Company</p>
              <a href="views/mentees.html">
                <li>Mentees</li>
              </a>
              <a href="https://spotknack.com/views/mission2021/">
                <li>Mission 2021</li>
              </a>
              <a href="views/campus_ambassadors/index.html" target="blank">
                <li>Campus Ambassadors</li>
              </a>

              <a href="views/startups.html" target="">
                <li>Spotknack for Startups</li>
              </a>
              <a href="views/educators.html" target="">
                <li>Spotknack for Educators</li>
              </a>
              <a href="views/donate.html" target="">
                <li>Donate</li>
              </a>
            </ul>
          </div>
          <div class="foot">
            <ul>
              <p>Featured On</p>
              <a
                href="https://www.edexlive.com/happening/2021/mar/17/heres-how-spotknack-is-securing-employment-opportunities-for-the-average-student-19088.html"
              >
                <li>Indian Express - Edex</li>
              </a>
            </ul>
          </div>
        </div>
        <!--Google map integration -->

        <div class="map">
          <ul>
            <p>Come meet us here</p>
            <iframe
              src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3915.4328324686107!2d76.98652631480348!3d11.081083792115216!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x0%3A0x5e517072b067391b!2siBevy+Forte!5e0!3m2!1sen!2sin!4v1562062625961!5m2!1sen!2sin"
              frameborder="0"
              style="border: 0"
              allowfullscreen
            ></iframe>
          </ul>
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
<style>
/*  footer */
.footer {
  padding-top: 100px;
  padding-bottom: 20px;
  width: 100%;
  background-color: #131415;
  height: auto;
}
.footer-line {
  display: flex;
  flex-direction: row;
  width: 100%;
}
.spot {
  padding-left: 5%;
}

.foot {
  width: 100%;
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
.map li {
  list-style-type: none;
}
.map iframe {
  border-radius: 20px;
  width: 70%;
  height: 60%;
}
.footer-content {
  width: 70%;
  display: flex;
  flex-direction: row;
  padding-left: 5%;
}

/*  social icons in the footer */

.social-icons {
  padding-left: 7.5%;
}
.icons a {
  padding-right: 2%;
}
.copyright {
  padding-left: 7.5%;
  padding-top: 1%;
}
.foot p {
  color: white;
  opacity: 0.3;
  font-size: 1.25rem;
  margin-top: 20px;
}
.map p {
  color: white;
  opacity: 0.3;
  font-size: 1.25rem;
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
    padding-left: 20%;
    width: auto;
  }

  .foot {
    /* padding-right:10%; */
    width: 100%;
  }
  .foot li {
    font-size: 1.7vw;
  }

  /* .footer-content {
    padding-left: 0;
  } */
}
@media only screen and (min-width: 768px) and (max-width: 1024px) {
  .foot li {
    font-size: 0.7rem;
  }
}
</style>
