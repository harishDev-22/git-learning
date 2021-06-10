<template>
  <div class="wrapper">
    <div class="flex-row-center-space-even web-banner">
      <div class="flex-col-center">
        <h2 class="info-header">Join hands to Empower 100 Students</h2>
        <p class="p-text text-center mt-10">
          Crowd Funding Campaign to help and impact 100 deserving students.
        </p>
        <form class="club-button">
          <script
            src="https://checkout.razorpay.com/v1/payment-button.js"
            data-payment_button_id="pl_GxWJx5s70ZnN0l"
            async
          ></script>
        </form>
      </div>

      <img
        class="mentoring-images"
        src="~assets/images/donate.png"
        width="100%"
        height="100%"
        alt="skillanalysis"
      />
    </div>
    <!--  How the fund will be utilized? -->
    <div class="feature-description">
      <h2 class="info-header">How the fund will be utilized?</h2>
      <!-- Feature description -->
      <p class="feature-description-content text-center mt-10">
        We are going to take care of every single rupee of the donors, it's our
        responsibility too. To bring in transparency, we will connect the donor
        with the student so that the donor would know for whom the money is
        being utilized and we are doing this not just for transparency, if the
        donors connected with the students, it would motivate the student for
        trusting them, to make use of the opportunity and make the donor feel
        that the money he/she donated is changing the student's life.
      </p>
    </div>
  </div>
</template>

<script>
export default {}
</script>
<style scoped>
.wrapper {
  margin-bottom: 10%;
}
.flex-row-center-space-even {
  margin: 11% 5% 15% 5%;
}

@media only screen and (min-width: 768px) and (max-width: 991px) {
  .flex-row-center-space-even {
    margin: 15% 5% 15% 5%;
  }
}
</style>
