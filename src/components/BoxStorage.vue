<template>
  <div class="hello">
    <div v-for="item in boxData" class="box"></div>
  </div>
</template>
<script>
export default {
  name: 'HelloWorld',
  data() {
    return {
      boxData:[],
    }
  },
  methods: {
    getData(){
      for(var a = 0; a<=9;a++){
        this.boxData.push(a)
      }
    }
  },
  mounted() {
    this.getData();
  },
}
</script>
<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.hello {
  position: fixed;
  display: flex;
  flex-wrap: wrap;
  width: 550PX;
  height: 380px;
  left: calc(50% - 275px);
  top: calc(50% - 190px);
}

.box {
  border: 2px solid rgb( 190, 240, 249);
  background-color: rgb(57, 146, 212);
  width: 100px;
  height: 180px;
  box-sizing: border-box;
  margin: 5px;
}
</style>
