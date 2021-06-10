<template>
  <div class="wrapper">
    <h1 class="info-header">Our Mentors</h1>
    <h2 class="sub-header-H2 poppins-font">
      Meet the people who make our journey awesome
    </h2>
    <div class="flex-wrap playfair-font">
      <div v-for="(n, $index) in 6" :key="$index" class="mentor-container">
        <img
          src="https://spotknackcompanywebsite.s3.us-east-2.amazonaws.com/images/ahielan.jpg"
          alt=""
          width="100%"
          height="95%"
        />
        <div class="text-center">
          <p class="name mt-22">Ahielan Ravichandran</p>
          <p class="career">Web Development Mentor</p>
          <p class="career">Software Engineer - Facilio Inc, Chennai</p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {}
</script>

<style scoped>
.wrapper {
  margin: 14.51% 0 14.51% 6%;
}
.flex-wrap {
  margin-top: 8%;
}
.mentor-container {
  margin-right: 6%;
  width: 26.8%;
  margin-bottom: 4.2%;
}
img {
  width: 100%;
  height: 500px;
}
h2 {
  font-weight: normal;
  margin-top: 50px;
}
.name,
.career {
  font-size: 16px;
  font-weight: bold;
  font-stretch: normal;
  font-style: normal;
  line-height: normal;
  letter-spacing: 0.6px;
  color: #000;
  padding: 0;
  margin-bottom: 0;
}
.career {
  opacity: 0.7;
  font-size: 12px;
  margin: 0;
  font-weight: normal;
}
@media screen and (max-width: 1291px) {
  img {
    height: auto;
  }
}
</style>
