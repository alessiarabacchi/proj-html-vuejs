<script>
export default {
  components: StatsSection,
};
</script>

<template>
  <section class="stats-text-split">
    <div class="text-section">
      <h2>EVERY MOMENT COUNTS</h2>
      <div class="underline"></div>
      <p>
        Curabitur non mi et turpis pharetra vulputate. Cras consequat, risus nec commodo vehicula, nisi est laoreet leo, ac convallis nisi nibh id velit. Aliquam mattis metus a nisi pretium.
      </p>
      <p>
        Lorem ipsum dolor sit amet, consectetur adipiscing elit. Praesent ac nibh vestibulum, laoreet ipsum quis, vestibulum nisi. Curabitur non mi et turpis pharetra vulputate. Ipsum dolor sit amet, consectetur adipiscing elit. Praesent ac nibh vestibulum, laoreet ipsum quis, vestibulum nisi.
      </p>
      <button class="mission-button">OUR MISSION</button>
    </div>
    <div class="stats-section">
      <div class="stat">
        <span class="stat-number">2032</span>
        <span class="stat-text">Volunteers worldwide</span>
      </div>
      <div class="stat">
        <span class="stat-number">132</span>
        <span class="stat-text">Active projects</span>
      </div>
      <div class="stat">
        <span class="stat-number">$3.8M</span>
        <span class="stat-text">Donated</span>
      </div>
    </div>
  </section>
</template>



<style lang="scss" scoped>
.stats-text-split {
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 2rem;
}
  .text-section {
    width: 50%;
    h2 {
      margin-bottom: 1rem;
    }
    .underline {
      width: 50px;
      height: 4px;
      background-color: #fec96b; 
      margin-bottom: 2rem;
    }
    .mission-button {
      background-color: #fec96b; 
      color: #fff;
      border: none;
      padding: 10px 20px;
      cursor: pointer;
      &:hover {
        background-color: darken(#fec96b, 10%);
      }
    }
  }

  .stats-section {
    width: 50%;
    background-color: #ed6865; 
    color: #fff;
    padding: 2rem;
    display: flex;
    flex-direction: column;
    align-items: flex-end;
    justify-content: center;
  }
    .stat {
      margin-bottom: 1rem;
    }
      .stat-number {
        font-size: 2rem;
        font-weight: bold;
      }