<template lang="">
  <div>
    <h4>{{ blog[0].title }}</h4>
    <p>{{blog[0].date}}</p>
  </div>
  <div>
    <h4>{{ blog[1].title }}</h4>
    <p>{{blog[1].date}}</p>
  </div>
  <div>
    <h4>{{ blog[2].title }}</h4>
    <p>{{blog[2].date}}</p>
  </div>
</template>
<script>
export default {
  name: "list",
  props: {
    blog : Array
  },
}
</script>
<style lang="">
  
</style>