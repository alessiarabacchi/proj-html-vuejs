<script>
export default {
  components: AppNavbar,
};
</script>

<template>
  <nav class="navbar">
    <div class="navbar-container">
      <a href="/" class="navbar-logo">
        <img src="./HelloIMG1669149314369.png" alt="AVADA CHARITY" />
      </a>
      <ul class="navbar-links">
        <li><a href="#home" class="nav-link">HOME</a></li>
        <li><a href="#mission" class="nav-link">MISSION</a></li>
        <li><a href="#causes" class="nav-link">CAUSES</a></li>
        <li><a href="#journal" class="nav-link">JOURNAL</a></li>
        <li><a href="#donate" class="nav-link donate">DONATE</a></li>
      </ul>
    </div>
  </nav>
</template>

<style lang="scss" scoped>
.navbar {
  background-color: transparent;
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 1rem 2rem;

  .navbar-container {
    width: 100%;
    max-width: 1200px;
    margin: 0 auto;
    display: flex;
    align-items: center;
    justify-content: space-between;
  }

  .navbar-logo {
    img {
      height: auto;
      width: 100px;
    }
  }

  .navbar-links {
    list-style: none;
    display: flex;
    margin: 0;
    padding: 0;

    .nav-link {
      text-decoration: none;
      color: #fff;
      margin-left: 2rem;
      padding: 0.5rem 1rem;
      transition: color 0.3s ease-in-out;

      &:hover {
        color: #aaa;
      }

      &.donate {
        background-color: #f1c40f;
        border-radius: 4px;
        color: #fff;

        &:hover {
          background-color: darken(#f1c40f, 10%);
        }
      }
    }
  }
}
</style>
