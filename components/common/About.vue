<template>
  <section class="about">
    <div class="main">
      <img class="img" src="~/assets/images/cec(1).png" alt="">
      <div class="about-text">
        <h1> <span class="red">H</span>akkımızda</h1>
        <h5><span class="red">K</span>TU <span class="red">C</span>EC Nedir?</h5>
        <p>
          Lorem ipsum dolor sit, amet consectetur adipisicing elit. Illo quis maiores repudiandae? Quos laudantium tempore ducimus modi, at deserunt! Mollitia rem labore sapiente dolorum placeat consequuntur recusandae iusto obcaecati quibusdam inventore amet quae eveniet, earum nemo molestias nulla laudantium nesciunt!
        </p>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: 'AboutComponent'
}
</script>

<style lang="scss" scoped>
@import "@/assets/scss/main.scss";
@import "@/assets/scss/colors.scss";

.about {
  width: 100%;
  padding: 78px 0px;
  background-color: $about-black;

  img {
    margin-right: 60px;
  }

  .main {
    width: 1130px;
    max-width: 95%;
    margin: 0 auto;
    display: flex;
    align-items: center;
    justify-content: space-around;

    .about-text {
      width: 550px;

      p{
        color: white;
        letter-spacing: 1px;
        line-height: 28px;
        font-size: 20px;
        margin-bottom: 45px;
      }

      h1{
        color: white;
        font-size: 80px;
        margin-bottom: 20px;
      }
      h5 {
        color: white;
        font-size: 27px;
        margin-bottom: 25px;
        letter-spacing: 2px;
      }
    }
  }

  img {
    height: auto;
    width: 400px;
    border: 1px solid black;
    border-radius: 50%;
  }
}

.red {
    color: $red;
}
</style>
