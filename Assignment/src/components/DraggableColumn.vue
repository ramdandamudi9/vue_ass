<template>
  <div class="col">
    <h3 class="col-heading">{{heading}}</h3>
    <draggable
            class="draggable-col"
            id="first"
            :list="list"
            :group="group"
    >
      <template #item="{ element }">
        <DraggableItem :item={element} />
      </template>
    </draggable>
  </div>
</template>

<script>
  import draggable from "vuedraggable";
  import DraggableItem from "./DraggableItem.vue"

  export default {
      components: {
          draggable,
          DraggableItem
      },
      props: {
          heading: String,
          list: Array,
          group: String
      }
  }
</script>

<style scoped>
  .col {
    text-align: center;
    flex: 1;
    margin: 0 10px;
    background-color:#dcf3f2;
  }

  .draggable-col {
    height: 50vh;
    overflow-y: scroll;
    padding: 0 50px;
  }

  .col-heading {
    color: dodgerblue;
  }
</style>
