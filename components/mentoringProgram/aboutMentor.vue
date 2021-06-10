<template>
  <div class="parent">
    <div class="program-description">
      <h2 class="sub-header-H2 text-left">Who is your mentor</h2>
      <p class="feature-description-content mt-22">
        {{ description }}
      </p>
    </div>
    <div v-if="topiclist" class="mt-22">
      <h4 class="sub-header-H4">Topics Overview</h4>
      <ul class="mentor-program-list mt-22">
        <li
          v-for="(topic, $topicIndex) in topiclist"
          :key="$topicIndex"
          class="feature-description-content mt-10"
        >
          {{ topic }}
        </li>
      </ul>
    </div>
    <div class="program-mentor-details mt-22">
      <h4 class="sub-header-H4">Career Mind Map Prepared with the help of</h4>
      <div class="flex-row-start mt-22">
        <img :src="mentorprofile.image" class="mentor-image-clip" alt="" />
        <div class="social-media-acccount">
          <div class="header-description-content">{{ mentorprofile.name }}</div>
          <div class="poppins-font-14 text-opacity">
            {{ mentorprofile.company }}
          </div>
          <div class="social-media-icons mt-05">
            <!----     <img src="../images/logo-facebook.svg" alt="">
                    <img style="background:dodgerblue ;" src="../images/logo-twitter.svg" alt=""> -->
            <a :href="mentorprofile.linkedInURL" target="_blank">
              <img
                src="https://spotknackcompanywebsite.s3.us-east-2.amazonaws.com/icons/linkedin.svg"
                alt="linkedin"
            /></a>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  props: {
    description: {
      type: String,
      default: '',
    },
    topiclist: {
      type: Array,
      default: null,
    },
    mentorprofile: {
      type: Object,
      default: null,
    },
  },
}
</script>
<style scoped>
.parent {
  margin-top: 20%;
}

.mentor-image-clip {
  width: 10%;
  border-radius: 33%;
}
.social-media-icons {
  width: 35px;
}
.social-media-acccount {
  margin-left: 15px;
}
</style>
