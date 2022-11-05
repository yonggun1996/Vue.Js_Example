<template>
    <div>
      <input type="radio" name="" id="html" value="HTML" v-model="favoriteLang">
      <label for="html">HTML</label>
    </div>
    <div>
      <input type="radio" name="" id="css" value="CSS" v-model="favoriteLang">
      <label for="css">CSS</label>
    </div>
    <div>
      <input type="radio" name="" id="js" value="JS" v-model="favoriteLang">
      <label for="js">js</label>
    </div>
    <div>선택한 지역: {{favoriteLang}}</div>
  </template>
  
  <script>
  export default {
      components: {},
      data() {
          return {
              favoriteLang: '' // 라디오는 하나만 선택할 수 있기 때문에 문자열로 바인딩을 해줘야 한다.
          }
      }
  }
  </script>
  
  <style>
  
  </style>