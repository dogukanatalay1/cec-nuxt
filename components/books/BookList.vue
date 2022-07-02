<template>
  <div class="books-container d-flex flex-column align-items-center">
    <div class="books-container-header">
      <h4 class="books-container-header-header">
        Alınmaya Hazır Kitaplarımız
      </h4>
    </div>
    <BooksBook v-for="book in books" :key="book.id" :book="book" />
  </div>
</template>

<script>
// import axios from 'axios'

export default {
  name: 'BookList',
  data () {
    return {
      books: []
    }
  },
  created () {
    this.getBooks()
  },
  methods: {
    getBooks () {
      this.$API.books.getBooks().then((response) => {
        this.books = response.data
      })
    }
    // async getBooks () {
    //   const data = axios.get(process.env.BASE_URL + 'books/')
    //   const result = await data

    //   this.books = result.data
    // }
  }
}
</script>

<style lang="scss" scoped>
@import '@/assets/scss/colors.scss';

.books-container {
  border: 1px solid black;
  width: 24%;
  border-radius: 12px;
  box-shadow: 4px 2px grey;
  transition: 0.4s;

  &:hover {
    box-shadow: 5px 3px $about-black;
    transition: 0.4s;
  }

  &-header {
    border: 1px solid black;

    &-header {
      border: 1px solid black;
    }
  }
}
</style>
