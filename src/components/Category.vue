<template>

  <div>
    <b-list-group >
       <b-list-group-item class="d-flex justify-content-between align-items-center lists">
       {{categories.name}}
       <!-- <b-badge variant="primary" pill>14</b-badge> -->
    </b-list-group-item>

    </b-list-group>
    
  </div>
    
</template>

<script>
export default {
  props: ['categories']
}
</script>

<style  scoped>
.lists{
  background-color: rgb(246, 240, 238);
  width: 100%;
}
</style>