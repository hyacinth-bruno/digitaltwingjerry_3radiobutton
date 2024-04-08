<template>
    <div class="feature-boxes">
      <div class="feature-box" v-for="n in 3" :key="n">
        <h3>Feature {{ n }}</h3>
        <div class="options">
          <input type="radio" :id="'option1-' + n" name="feature" value="Option 1">
          <label :for="'option1-' + n">Option 1</label>
          <input type="radio" :id="'option2-' + n" name="feature" value="Option 2">
          <label :for="'option2-' + n">Option 2</label>
          <input type="radio" :id="'option3-' + n" name="feature" value="Option 3">
          <label :for="'option3-' + n">Option 3</label>
        </div>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    name: 'FeatureBox',
  };
  </script>
  
  <style scoped>
  .feature-boxes {
    display: flex;
    flex-direction: column; /* Change to column for vertical alignment */
    align-items: center; /* Center align the feature boxes */
    padding: 20px;
  }
  
  .feature-box {
    border: 2px solid darkblue;
    border-radius: 10px;
    padding: 20px;
    margin: 10px;
    background-color: lightblue; /* Change background color to light blue */
    width: 30%; /* Adjust width as necessary for design */
  }
  </style>
  