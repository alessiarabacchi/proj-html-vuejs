<script>
export default {
  components: ArticlesSection,
  data() {
    return {
      articles: [
        {
          id: 1,
          title: "The human story of uniqueness",
          summary: "Lorem ipsum dolor sit amet, consectetur adipiscing elit...",
          image: "proj-html-vuejs/src/components/HelloIMG1669149322752.jpeg",
        },
        {
          id: 2,
          title: "Sustainable trade tactics",
          summary: "Lorem ipsum dolor sit amet, consectetur adipiscing elit...",
          image: "proj-html-vuejs/src/components/HelloIMG1669149322752.jpeg",
        },
        {
          id: 3,
          title: "Farmers making a difference",
          summary: "Lorem ipsum dolor sit amet, consectetur adipiscing elit...",
          image: "proj-html-vuejs/src/components/HelloIMG1669149322752.jpeg",
        },
        {
          id: 4,
          title: "Meeting remote tribus in Peru",
          summary: "Lorem ipsum dolor sit amet, consectetur adipiscing elit...",
          image: "proj-html-vuejs/src/components/HelloIMG1669149322752.jpeg",
        },
        {
          id: 5,
          title: "Understanding community compiexities",
          summary: "Lorem ipsum dolor sit amet, consectetur adipiscing elit...",
          image: "proj-html-vuejs/src/components/HelloIMG1669149322752.jpeg",
        },
      ],
    };
  },
};
</script>

<template>
  <section class="latest-articles">
    <div class="section-header">
      <h2>LATEST ARTICLES</h2>
      <p>Together we make all the difference</p>
    </div>
    <div class="articles-grid">
      <article
        class="article-card"
        v-for="article in articles"
        :key="article.id"
      >
        <img :src="article.image" :alt="article.title" class="article-image" />
        <h3 class="article-title">{{ article.title }}</h3>
        <p class="article-summary">{{ article.summary }}</p>
      </article>
    </div>
    <button class="view-all-button">VIEW ALL OUR ARTICLES</button>
  </section>
</template>

<style lang="scss" scoped>
.articles-section {
  display: flex;
  flex-wrap: wrap;
  justify-content: space-between;
  margin: 2rem;

  .article {
    width: 30%;
    margin-bottom: 2rem;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
    transition: box-shadow 0.3s ease-in-out;

    &:hover {
      box-shadow: 0 6px 12px rgba(0, 0, 0, 0.2);
    }

    .article-image {
      width: 100%;
      height: auto;
      border-top-left-radius: 4px;
      border-top-right-radius: 4px;
    }

    .article-content {
      padding: 1rem;

      .article-title {
        font-size: 1.2rem;
        margin-bottom: 0.5rem;
      }

      .article-description {
        font-size: 1rem;
        color: #666;
        margin-bottom: 1rem;
      }

      .article-link {
        font-size: 1rem;
        color: #0056b3;
        text-decoration: none;

        &:hover {
          text-decoration: underline;
        }
      }
    }
  }
}
</style>
