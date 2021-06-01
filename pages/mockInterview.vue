<template>
  <div>
    <div class="body-content">
      <div class="box-content-body">
        <div class="box-content-finder flex-col-center">
          <h2 class="playfair-font">Mock Interview</h2>
          <p class="p-text">
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
    </div>
  </div>
</template>

<script>
export default {}
</script>
<style scoped>
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
  padding-top: 10%;
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
</style>
