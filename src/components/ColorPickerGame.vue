<template>
    <h1 className="name" >Color Picker Game</h1>
  
    <div className = "message" >{{ message }}</div>

    <button className="btn" v-for="color in colours" :key="color" @click="matchColour(color)">{{ color }}</button>
  
   
  </template>
  
  <script>
  import colourPicker from "@/composable/color-picker";
  
  export default {
  
    name: "ColorPickerGame",
  
    setup() {
     
      const { colours, message, matchColour } = colourPicker();
  
      
      return { colours, message, matchColour };
    },
  };
  </script>
  
  <style>
    .name {
     color: goldenrod;
     font-size: 5rem;
    }

   .message{
    padding-bottom: 6rem;
    font-size: 1.5rem;
   } 

   .btn{
    padding: 2rem ;
    border-radius: 50%;
    font-size: 2rem;
    width: 9rem;
    margin: 0 2rem;
    gap: 1;
    justify-content: center;
   }
  </style>
  