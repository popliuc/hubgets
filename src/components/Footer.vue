<template>
  <div class="footer footer-grid">
    <div class="first-column">
      <div>
        <img class="hubgets-logo" alt="HubGets logo" src="./../assets/hubgets-logo.png" />
      </div>
    </div>
    <div class="second-column">
      <div>
        <div class="footer-section-title">
          <b>OUR COMPANY</b>
        </div>
        <div class="link-data">
          <a class="html-link opacity" href="#">About us</a>
        </div>
        <div class="link-data">
          <a class="html-link opacity" href="#">Blog</a>
        </div>
        <div class="link-data">
          <a class="html-link opacity" href="#">We are hiring</a>
        </div>
        <div class="link-data">
          <a class="html-link" href="#">Terms of service</a>
        </div>
        <div class="link-data">
          <a class="html-link opacity" href="#">Contact us</a>
        </div>
      </div>
    </div>
    <div class="third-column">
      <div>
        <div class="footer-section-title">
          <b>HUBGETS</b>
        </div>
        <div class="link-data">
          <a class="html-link opacity" href="#">Join the program</a>
        </div>
        <div class="link-data">
          <a class="html-link opacity" href="#">Features</a>
        </div>
        <div class="link-data">
          <a class="html-link opacity" href="#">Curent status</a>
        </div>
      </div>
    </div>
    <div class="fourth-column">
      <div>
        <div class="footer-section-title">
          <b>SOCIAL</b>
        </div>
        <div class="link-data">
          <a class="html-link opacity" href="#">
            <img class="social-logo" alt="Twitter logo" src="./../assets/twitter.png" />
            Twitter
          </a>
        </div>
        <div class="link-data">
          <img class="social-logo" alt="Youtube logo" src="./../assets/youtube.png" />
          <a class="html-link opacity" href="#">Youtube</a>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {};
</script>
<style scoped>
.footer {
  background: #0070bb;
  color: white;
}
.footer-grid {
  display: grid;
  grid-template-columns: 20% 15% 15% 15% 15% 20%;
  align-items: top;
  font-size: 14px;
}
.first-column {
  grid-column-start: 2;
  grid-column-end: 2;
  grid-row-end: 1;
  grid-row-start: 1;
  margin: 10px;
}
.second-column {
  grid-column-start: 3;
  grid-column-end: 3;
  grid-row-end: 1;
  grid-row-start: 1;
  margin: 10px;
}

.third-column {
  grid-column-start: 4;
  grid-column-end: 4;
  grid-row-end: 1;
  grid-row-start: 1;
  margin: 10px;
}
.fourth-column {
  grid-column-start: 5;
  grid-column-end: 5;
  grid-row-end: 1;
  grid-row-start: 1;
  margin: 10px;
}

@media screen and (max-width: 900px) {
  .footer-grid {
    display: grid;
    grid-template-columns: 50% 50%;
    align-items: top;
    font-size: 14px;
  }
  .first-column {
    grid-column-start: 1;
    grid-column-end: 1;
    grid-row-end: 1;
    grid-row-start: 1;
    margin: 10px;
  }
  .second-column {
    grid-column-start: 2;
    grid-column-end: 2;
    grid-row-end: 1;
    grid-row-start: 1;
    margin: 10px;
  }

  .third-column {
    grid-column-start: 1;
    grid-column-end: 1;
    grid-row-end: 2;
    grid-row-start: 2;
    margin: 10px;
  }
  .fourth-column {
    grid-column-start: 2;
    grid-column-end: 2;
    grid-row-end: 2;
    grid-row-start: 2;
    margin: 10px;
  }
}

.html-link {
  color: inherit;
  text-decoration: unset;
}
.opacity {
  opacity: 0.4;
}
.link-data {
  margin-bottom: 5px;
  text-align: left;
}
.footer-section-title {
  text-align: left;
  margin-bottom: 8px;
  margin-top: 20px;
}
.hubgets-logo {
  height: 20px;
}
.social-logo {
  height: 20px;
  width: 20px;
  vertical-align: text-top;
}
</style>