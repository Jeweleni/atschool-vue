<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <p>
      Hello Ikenna, nice to meet you
    </p>
    <p>{{count}}</p>
    <button @click="incrementCount">Increment</button>
  </div>
</template>

<script>

export default {
  name: 'HelloWorld',
  props: {
    msg: String
  },
  data(){
    return{
      count: 12 ,
    };
  },



methods:{
  incrementCount() {
    this.count++;
  },
},

beforeCreate(){
  console.log("beforeCreate has been calledd")
},

created(){
  console.log("created has been called")
},

beforeMount(){
  console.log("beforeMount has been called")
},

mounted(){
  console.log("mounted has been called")
},

beforeUpdate(){
  console.log("beforeUpdate has been called")
},

updated(){
  console.log("update has been called")
},
};
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
</style>
