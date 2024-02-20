<script>
export default {
  components: AppFooter
};
</script>

<template>
    <footer class="footer">
      <div class="footer-content">
        <a href="/" class="footer-logo">
          <img src="HelloIMG1669149323379.png" alt="AVADA CHARITY" /> 
        </a>
        <div class="footer-rights">
          <p>&copy; 2024 AVADA CHARITY. All Rights Reserved | Powered by WordPress</p>
        </div>
        <div class="footer-social">
          <a href="https://facebook.com" target="_blank" class="social-link">
            <img src="./facebook1.png" alt="Facebook" />

          <a href="https://instagram.com" target="_blank" class="social-link">
            <img src="./instagram.svg" alt="Instagram" /> 
          </a>
          <a href="https://twitter.com" target="_blank" class="social-link">
            <img src="./twitter.png" alt="Twitter" /> 
          </a>
          <a href="https://youtube.com" target="_blank" class="social-link">
            <img src="./youtube.png" alt="YouTube" /> 
          </a>
        </div>
      </div>
    </footer>
  </template>
  
 
  
  <style lang="scss" scoped>
  .footer {
    background-color: #f9f9f9;
    padding: 2rem 0;
    display: flex;
    align-items: center;
    justify-content: space-between;
  
    .footer-content {
      display: flex;
      justify-content: space-between;
      align-items: center;
      width: 100%;
      max-width: 1200px;
      margin: 0 auto;
      padding: 0 1rem;
  
      .footer-logo {
        display: flex;
        align-items: center;
  
        img {
          height: auto;
          width: 100px; 
        }
      }
  
      .footer-rights {
        text-align: center;
        flex: 1;
        font-size: 0.875rem;
        color: #333;
        margin: 0 2rem;
  
        p {
          margin: 0;
        }
      }
  
      .footer-social {
        display: flex;
        color: goldenrod;
        
        .social-link {
          display: inline-block;
          margin-left: 1rem;
  
          img {
            height: auto;
            width: 20px; 
          }
        }
      }
    }
  }
  </style>