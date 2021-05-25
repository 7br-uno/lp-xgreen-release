<template>
  <div>
    <h1 class="example">{{ hello_world }}</h1>
    <exampleComponent />
    <v-btn
      elevation="2"
      color="blue"
      @click="hello_daniel()"
      dark
    >Click me</v-btn>
    
  </div>
</template>

<script>
  import exampleComponent from '/components/example_component';
  export default{
    components:{
      exampleComponent
    },
    data: () => {
      return {
        hello_world: 'Hello World',
        daniel_name: 'Daniel',
        counter: 0
      }
    },
    mounted(){
      this.hello_daniel(); //Chama a função hello_daniel() quando a página é montada
    },
    methods:{
      hello_daniel(){
        console.log('Hello ' + this.daniel_name);
        console.log(this.counter ++);
      }
    }
  }
</script>

<style scoped>
.example{
  color: red;
}
</style>