<script>
  export default{
    data:() => ({
      contador: 10,
    }),
    methods:{
      incrementar(){
        this.contador++;
      },
      disminuir(){
        this.contador--;
      },
      reset(){
        this.contador=10;
      },
    }
  };
</script>
<template>
  <img src="./assets/logo.svg" alt="logo VUE" width="125" height="125">
  <div class="container">
    <small>
      <h1>hola desde vue</h1>
    </small>
  <hr>
  <h2>contador {{contador}}</h2>
  <button @click="incrementar()">+1</button>
  <button @click="disminuir()">-1</button>
  <button @click="reset">reset</button>
  </div>
</template>

<style scoped>
  .container{
    text-align: center;
  }
  small{
    color: #666;
  }
  h1 {
    font-weight: bolder;
  }
  h2{
    color:black
  }
  button {
  cursor : pointer ;
  font-size : 1.5rem ;
  margin : 0px 8px ;
  }
</style>