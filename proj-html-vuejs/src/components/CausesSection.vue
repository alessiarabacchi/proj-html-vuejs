<script>
export default {
  name: "RecentCausesSection",
  data() {
    return {
      causeImages: [
        {
          id: 1,
          src: "proj-html-vuejs/src/components/HelloIMG1669149317319.jpeg",
          alt: "Description of Image 1",
        },
        {
          id: 2,
          src: "proj-html-vuejs/src/components/HelloIMG1669149318263.jpeg",
          alt: "Description of Image 2",
        },
        {
          id: 3,
          src: "proj-html-vuejs/src/components/HelloIMG1669149319450.jpeg",
          alt: "Description of Image 3",
        },
        {
          id: 4,
          src: "proj-html-vuejs/src/components/HelloIMG1669149321401.jpeg",
          alt: "Description of Image 4",
        },
      ],
    };
  },
};
</script>

<template>
  <section class="recent-causes">
    <div class="section-header">
      <h2>RECENT CAUSES</h2>
      <p>We run projects in over 30 countries in 5 continents</p>
    </div>
    <div class="causes-images">
      <div class="cause-image" v-for="image in causeImages" :key="image.id">
        <img :src="image.src" :alt="image.alt" />
      </div>
    </div>
    <button class="view-all-button">VIEW ALL OUR CAUSES</button>
  </section>
</template>

<style lang="scss" scoped>
.recent-causes {
  background-color: #fff;
  padding: 2rem;
  text-align: center;

  .section-header {
    margin-bottom: 2rem;

    h2 {
      font-size: 2rem;
      margin-bottom: 0.5rem;
    }

    p {
      color: #555;
      margin-bottom: 2rem;
    }
  }

  .causes-images {
    display: flex;
    justify-content: space-between;
    margin-bottom: 2rem;

    .cause-image {
      width: calc(25% - 1rem);
      margin: 0 0.5rem;

      img {
        width: 100%;
        height: auto;
        border-radius: 4px;
      }
    }
  }

  .view-all-button {
    background-color: #f04e30;
    color: #fff;
    border: none;
    padding: 1rem 2rem;
    cursor: pointer;
    border-radius: 2px;
    font-size: 1rem;
    transition: background-color 0.3s;

    &:hover {
      background-color: darken(#f04e30, 10%);
    }
  }
}
</style>
