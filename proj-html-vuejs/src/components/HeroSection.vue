<script>
export default {
  name: 'HeroSection',
  methods: {
    goToMission() {
      
    },
    goToDonate() {
      
    },
  },
};
</script>

<template>
  <section class="hero-section" style="background-image: url('./HelloIMG1669149393797.jpeg');">
    <div class="hero-content">
      <h1 class="hero-title">MAKE A DIFFERENCE</h1>
      <p class="hero-subtitle">As long as poverty, injustice & inequality persist, none of us can truly rest.</p>
      <div class="hero-cta">
        <button @click="goToMission" class="hero-button mission">OUR MISSION</button>
        <button @click="goToDonate" class="hero-button donate">DONATE NOW</button>
      </div>
    </div>
  </section>
</template>



<style lang="scss" scoped>
.hero-section {
  display: flex;
  align-items: center;
  justify-content: center;
  text-align: center;
  background-size: cover;
  background-position: center;
  height: 100vh; 

  .hero-content {
    color: #fff;
    max-width: 600px;
    padding: 2rem;

    .hero-title {
      font-size: 2.5rem;
      margin-bottom: 1rem;
    }

    .hero-subtitle {
      font-size: 1.25rem;
      margin-bottom: 2rem;
    }

    .hero-cta {
      .hero-button {
        padding: 1rem 2rem;
        margin-right: 1rem;
        border: none;
        border-radius: 2px;
        font-size: 1rem;
        cursor: pointer;
        transition: background-color 0.3s;

        &.mission {
          background-color: #eee; 
          color: #333;

          &:hover {
            background-color: darken(#eee, 10%);
          }
        }

        &.donate {
          background-color: #ffa500; 
          color: #fff;

          &:hover {
            background-color: darken(#ffa500, 10%);
          }
        }
      }
    }
  }
}