<template>
  <div class="list-item">
    {{ item.element }}
  </div>
</template>

<script>
  export default {
      props: {
          item: String
      }
  }
</script>

<style scoped>
  .list-item{
    background-color: white;
    padding: 5px;
    border-radius: 8px;
    margin: 4px auto;
    box-shadow: #a4abaa 3px 3px 5px;
    min-width: 150px;
    width: max-content;
    cursor: pointer;
  }
</style>
