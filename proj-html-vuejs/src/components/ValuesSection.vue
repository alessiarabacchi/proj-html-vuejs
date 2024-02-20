<script>
export default {
  name: "ValuesSection",
  data() {
    return {
      values: [
        {
          title: "Clean Water",
          description: "Description of Clean Water value...",
          icon: "proj-html-vuejs/src/components/drop_icon-icons.com_54400.png",
        },
        {
          title: "Vaccinations",
          description: "Description of Vaccinations value...",
          icon: "proj-html-vuejs/src/components/vaccino.png",
        },
        {
          title: "Education",
          description: "Description of Education value...",
          icon: "proj-html-vuejs/src/components/education.png",
        },
        {
          title: "Farming",
          description: "Description of Farming value...",
          icon: "proj-html-vuejs/src/components/farming.png",
        },
      ],
    };
  },
};
</script>

<template>
  <section class="values-section">
    <div class="values-header">
      <h2>OUR VALUES</h2>
      <p>Think Big. Act Bigger.</p>
    </div>
    <div class="values-grid">
      <div class="value-card" v-for="value in values" :key="value.title">
        <img :src="value.icon" :alt="value.title" class="value-icon" />
        <h3 class="value-title">{{ value.title }}</h3>
        <p class="value-text">{{ value.description }}</p>
        <button class="learn-more-btn">LEARN MORE</button>
      </div>
    </div>
  </section>
</template>

<style lang="scss" scoped>
.values-section {
  background-color: url(./HelloIMG1669149393797.jpeg);
  text-align: center;
  padding: 4rem 0;

  .values-header {
    margin-bottom: 3rem;

    h2 {
      font-size: 2.5rem;
      margin-bottom: 0.5rem;
    }

    p {
      font-size: 1.5rem;
      color: #666;
    }
  }

  .values-grid {
    display: flex;
    justify-content: space-around;
    gap: 2rem;

    .value-card {
      width: 22%;
      padding: 2rem;
      border-radius: 4px;
    }
    .value-icon {
      width: 100px;
      height: auto;
      margin-bottom: 1rem;
    }

    .value-title {
      font-size: 1.5rem;
      color: #333;
      margin-bottom: 0.5rem;
    }

    .value-description {
      font-size: 1rem;
      color: #666;
    }
  }
}
</style>
