<template>
  <div>
    <BookList />
  </div>
</template>

<script>
import BookList from '../components/books/BookList.vue'
export default {
  name: 'TestVue',
  components: { BookList },
  data () {
    return {}
  }
}
</script>
