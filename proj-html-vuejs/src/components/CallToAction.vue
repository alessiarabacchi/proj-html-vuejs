<script>
export default {
  components: CallToAction,
  methods: {
    goToVolunteer() {},
    goToDonate() {},
  },
};
</script>

<template>
  <section
    class="cta-section"
    style="background-image: url(./HelloIMG1669149393797.jpeg)"
  >
    <div class="cta-content">
      <h2 class="cta-title">CHANGE A LIFE TODAY</h2>
      <p class="cta-text">
        As long as poverty, injustice & inequality persist, none of us can truly
        rest. It doesn't take much to change a life. Get in touch today and
        start making the difference.
      </p>
      <div class="cta-buttons">
        <button @click="goToVolunteer" class="cta-button volunteer">
          VOLUNTEER
        </button>
        <button @click="goToDonate" class="cta-button donate">
          DONATE NOW
        </button>
      </div>
    </div>
  </section>
</template>

<style lang="scss" scoped>
.cta-section {
  display: flex;
  align-items: center;
  justify-content: center;
  background-size: cover;
  background-position: center;
  text-align: center;
  padding: 4rem 0;

  .cta-content {
    color: #fff;
    max-width: 600px;

    .cta-title {
      font-size: 3rem;
      margin-bottom: 1rem;
    }

    .cta-text {
      margin-bottom: 2rem;
    }

    .cta-buttons {
      .cta-button {
        padding: 1rem 2rem;
        margin: 0 0.5rem;
        border: 2px solid #fff;
        background: none;
        color: #fff;
        font-size: 1rem;
        cursor: pointer;
        transition: all 0.3s ease;

        &.volunteer:hover,
        &.donate:hover {
          background: #fff;
          color: #000;
        }
      }
    }
  }
}
</style>
