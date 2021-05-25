<template>
  <div>
    <h1 class="example">{{ hello_world }}</h1>
    <v-btn
      elevation="2"
      color="blue"
      @click="hello_daniel()"
      dark
    >Click me</v-btn>
  </div>
</template>

<script>
  export default{
    data: () => {
      return {
        hello_world: 'Hello World',
        daniel_name: 'Daniel'
      }
    },
    mounted(){
      this.hello_daniel();
    },
    methods:{
      hello_daniel(){
        console.log('Hello ' + this.daniel_name);
      }
    }
  }
</script>

<style scoped>
.example{
  color: red;
}
</style>