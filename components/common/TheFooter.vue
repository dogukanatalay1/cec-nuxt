<template>
  <footer class="footer-distributed">
    <div class="footer-left">
      <!--  <img src="@/assets/images/cecicon.jpg"> -->
      <h3 class="mt-4 ml-5">
        KTU<span>CEC</span>
      </h3>

      <p class="footer-company-name ml-5" style="color: #fff; font-size: 20px">
        Aramıza Hoşgeldin!
      </p>
    </div>

    <div class="footer-center">
      <div>
        <i class="fa fa-map-marker" />
        <p>
          <span>Trabzon Kanuni Kampüsü Bilgisayar Mühendisliği Bölüm Binası</span>
          Trabzon, bla bla - 61000
        </p>
      </div>

      <div>
        <i class="fa fa-phone" />
        <p>+5xx xxx xx xx</p>
      </div>
      <div>
        <i class="fa fa-envelope" />
        <p><a href="mailto:support@eduonix.com">ktucec@gmail.com</a></p>
      </div>
    </div>
    <div class="footer-right">
      <p class="footer-company-about">
        <span>KTUCEC Hakkında</span>
        Lorem ipsum dolor sit amet consectetur, adipisicing elit. Culpa laborum
        in, velit iusto vel saepe.
      </p>
      <div class="footer-icons">
        <a
          class="icon"
          href="https://twitter.com/ktucec"
          target="_blank"
        ><ion-icon name="logo-twitter" /></a>
        <a
          class="icon"
          href="https://www.instagram.com/ktucec/"
          target="_blank"
        ><ion-icon name="logo-instagram" /></a>
        <a
          class="icon"
          href="https://www.linkedin.com/in/ktucec/"
          target="_blank"
        ><ion-icon name="logo-linkedin" /></a>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  data () {
    return {}
  }
}
</script>

<style lang="scss" scoped>
@import '@/assets/scss/colors.scss';
@import '@/assets/scss/main.scss';

/* #150000 30%, #3f0000 */
/* @/assets/images/cecicon.jpg */

footer {
  position: fixed;
  bottom: 0;
  box-sizing: border-box;
}

@media (max-height: 800px) {
  footer {
    position: static;
  }
  header {
    padding-top: 40px;
  }
}

.footer-distributed {
  background: linear-gradient(to right, #150000 40%, #3f0000);
  box-sizing: border-box;
  width: 100%;
  position: absolute;
  bottom: 0;
  text-align: left;
  font: bold 16px sans-serif;
  padding: 50px 50px 60px 50px;
  border-top-left-radius: 130px;
  margin-top: 80px;
}

.footer-distributed .footer-left,
.footer-distributed .footer-center,
.footer-distributed .footer-right {
  display: inline-block;
  vertical-align: top;
  box-sizing: border-box;
}

/* Footer left */

.footer-distributed .footer-left {
  width: 30%;
}

.footer-distributed h3 {
  color: #ffffff;
  font: normal 36px 'Cookie', cursive;
  margin: 0;
}

/* The company logo */

.footer-distributed .footer-left img {
  width: 30%;
}

.footer-distributed h3 span {
  color: $red;
}

/* Footer links */

.footer-distributed .footer-links {
  color: #ffffff;
  margin: 20px 0 12px;
}

.footer-distributed .footer-links a {
  display: inline-block;
  line-height: 1.8;
  text-decoration: none;
  color: inherit;
}

.footer-distributed .footer-company-name {
  color: #8f9296;
  font-size: 14px;
  font-weight: normal;
  margin: 0;
}

/* Footer Center */

.footer-distributed .footer-center {
  width: 35%;
}

.footer-distributed .footer-center i {
  background-color: #33383b;
  color: #ffffff;
  font-size: 25px;
  width: 38px;
  height: 38px;
  border-radius: 50%;
  text-align: center;
  line-height: 42px;
  margin: 10px 15px;
  vertical-align: middle;
}

.footer-distributed .footer-center i.fa-envelope {
  font-size: 17px;
  line-height: 38px;
}

.footer-distributed .footer-center p {
  display: inline-block;
  color: #ffffff;
  vertical-align: middle;
  margin: 0;
}

.footer-distributed .footer-center p span {
  display: block;
  font-weight: normal;
  font-size: 14px;
  line-height: 2;
}

.footer-distributed .footer-center p a {
  color: $red;
  text-decoration: none;
}

/* Footer Right */

.footer-distributed .footer-right {
  width: 30%;
}

.footer-distributed .footer-company-about {
  line-height: 20px;
  color: #92999f;
  font-size: 13px;
  font-weight: normal;
  margin: 0;
}

.footer-distributed .footer-company-about span {
  display: block;
  color: #ffffff;
  font-size: 18px;
  font-weight: bold;
  margin-bottom: 20px;
}

.footer-distributed .footer-icons {
  margin-top: 25px;
  box-sizing: border-box;
}

.footer-distributed .footer-icons a {
  display: inline-block;
  width: 35px;
  height: 35px;
  cursor: pointer;
  border-radius: 2px;

  font-size: 20px;
  color: #ffffff;
  text-align: center;
  line-height: 35px;
}

.footer-distributed .footer-icons a:hover {
  color: red;
}

/* Here is the code for Responsive Footer */
/* You can remove below code if you don't want Footer to be responsive */

@media (max-width: 880px) {
  .footer-distributed .footer-left,
  .footer-distributed .footer-center,
  .footer-distributed .footer-right {
    display: block;
    width: 100%;
    margin-bottom: 40px;
    text-align: center;
  }

  .footer-distributed .footer-center i {
    margin-left: 0;
  }
}
</style>
