<template>
    <h1>Color Picker Game</h1>
  
    <div>{{ message }}</div>

    <button v-for="color in colours" :key="color" @click="matchColour(color)">{{ color }}</button>
  
   
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
  
  <style></style>
  