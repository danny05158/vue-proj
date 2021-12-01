<template>
  <draggable @start="drag=true" @end="drag=true" class="dragArea">
      <div v-for="(item, index) in icons" :key="index" class="icon-container">
         <img  alt="icon-img" class="icon-img" src="../assets/nav.png" />
          <p>{{ item.name }}</p>
      </div>
  </draggable>
</template>

<script>
import draggable from "vuedraggable";

export default {
  name: 'Icons',
    components: {
    draggable
  },
  data: function() {
    return {
      icons:[
        {name: "Title 1"}, {name: "Title 2"}, {name: "Title 3"}, {name: "Title 4"}, {name: "Title 5"},{name: "Title 6"}
      ]
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

.dragArea {
  display: flex;
  margin: 0 51px;
}

.icon-container{
  display: flex;
  flex-flow: column;
  align-items: center;
}

.icon-img{
  width: 80px;
  height: 80px;
  max-width: 100%;
}

</style>
