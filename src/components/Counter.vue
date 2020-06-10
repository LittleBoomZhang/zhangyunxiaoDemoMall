<template>
    <div>
      <button @click="increment">+</button>
      <button v-on:click="decrement">-</button>
      <p><span>{{num}}</span></p>
    </div>
</template>

<script>
    export default {
      name: "Counter",
      props: ['num'],
      data(){
        return {

        }
      },
      methods:{
        increment(){
          this.$emit("incre");
        },

        decrement(){
          this.$emit("decre");
        }
      }
    }
</script>

<style scoped>

</style>
