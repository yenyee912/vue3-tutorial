<template>
<div class="mt-2">

<b-icon icon="archive" scale="2" @click="increaseCount" >click me</b-icon>
<br />

<b-btn @click="showOverlay= !showOverlay">Convert true/false</b-btn>  
showOverlay: {{showOverlay}}
  

  
</div>
  
</template>

<script>
export default {
  data(){
    return{
      showOverlay: false,
      buttonSize: "lg",

      fruits: ["apple", "orange", "pear", "durian"],

      apple: {
        name: "Fuji",
        price: "1",
        color: "red"
      },

      // object array
      products: [
        {
          name: "Apple",
          quantity: 0,
          price: 10,
          stock: 0,
          image: "apple.jpg",
          url: "https://www.google.com"
        },
        {
          name: "Orange",
          quantity: 0,
          price: 12,
          stock: 0,
          image: "orange.jpg",
          url: "https://www.facebook.com"

        },
        {
          name: "Strawberry",
          quantity: 0,
          price: 9,
          stock: 0,
          url: "https://www.discord.com"
        },
        {
          name: "Strawberry 2",
          quantity: 0,
          price: 7,
          stock: 0,
          image: "strawberry.jpeg",
        },
        {
          name: "Orange 2",
          quantity: 0,
          price: 13,
          stock: 0,
          image: "orange.jpg",
        },
        {
          name: "Apple 2",
          quantity: 0,
          price: 11,
          stock: 0,
          image: "apple.jpg",
        },
      ],

      
      
    }
  },

  methods:{
    increaseCount(){
      console.log('me!!')
    },
    iterateLoop(){
      let arr= [1, 2, 3]

      for (let i=0; i<arr.length; i++){
        console.log(arr[i])
      }

    }
  }

}
</script>

<style>

</style>