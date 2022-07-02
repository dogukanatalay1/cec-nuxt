<template>
  <div class="book d-flex flex-row align-items-center justify-content-around">
    <div class="book-img">
      <div class="img">
        <img src="@/assets/images/cec(1).png" alt="">
      </div>
    </div>
    <div class="book-name">
      <span>{{ book.title }}</span>
    </div>
  </div>
</template>

<script>
export default {
  name: 'BookCard',
  props: {
    book: {
      type: Object,
      required: true
    }
  }
}
</script>

<style lang="scss" scoped>
@import '@/assets/scss/colors.scss';

.book {
  border: 1px solid black;
  width: 260px;
  height: 10vh;
  margin: 8px;
  padding: 5px;
  border-radius: 4px;
  box-shadow: 4px 2px grey;
  background-color: $red;
  transition: 0.4s;

  &:hover {
    box-shadow: 5px 3px $about-black;
    transition: 0.4s;
    transform: scale(1.02);
  }

  &-img {
    border: 1px solid black;
    width: 24%;
    height: 80%;

    img {
      background-size: cover;
      width: 100%;
      height: 100%;
    }
  }

  &-name {
    border: 1px solid black;
    width: 60%;
    // ellipsis
    color: #fff;
  }
}
</style>
