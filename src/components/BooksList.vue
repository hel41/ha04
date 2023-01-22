<template>
  <div id="books" v-for="i in size" :key="i" >
    <div class="book">
      <div class="book-title" >
        {{value[i-1].title }}</div>
      <div class="book-author">
        {{value[i-1].authors }}
      </div>
    </div>
    
  </div>
  <!-- TODO: implement me -->
  <img src='@/assets/BooksList.jpg' class='img-fluid rounded' alt=''>
</template>

<script>
export default {
  name: 'BooksList',
  props:['value', 'size']

}
</script>
<!-- !!! Achtung nur zu testzwecken eingefügt !!!! André -->
<style>
  .book-title{
    font-size: 1em;
    font-weight: bold;
}
  .book-author{
    font-size: 0.6em;
    font-style: italic;
    margin-left: 10px;
  }
#books{
 border:0.3px solid rgb(166, 165, 165);
 padding: 15px
}
</style>