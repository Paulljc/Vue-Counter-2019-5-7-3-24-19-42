<template>
  <div class="hello">
    <button @click="decrease"> - </button>
      <span class="number">{{ count }}</span>
    <button @click="increase"> + </button>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data() {
    return {
      count: 0
    }
  },
  methods:{
    decrease(){
      this.count--;
    },
    increase(){
      this.count++;
    }
  },
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
.number {
  margin: 10px;
}
</style>
