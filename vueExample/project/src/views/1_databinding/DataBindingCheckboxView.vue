<template>
  <div>
    <input type="checkbox" name="" id="html" value="HTML" v-model="favoriteLang">
    <label for="html">HTML</label>
  </div>
  <div>
    <input type="checkbox" name="" id="css" value="CSS" v-model="favoriteLang">
    <label for="css">CSS</label>
  </div>
  <div>
    <input type="checkbox" name="" id="js" value="JS" v-model="favoriteLang">
    <label for="js">js</label>
  </div>
  <div>선택한 지역: {{favoriteLang}}</div>
  <!-- checked값이 t/f인지 사용자가 조작을 하기 때문에 checked와 데이터바인딩이 된다. -->
  <!-- 그래서 checked가 된 값의 value를 가져온다. -->
</template>

<script>
export default {
    components: {},
    data() {
        return {
            favoriteLang: ['CSS']
        }
    }
}
</script>

<style>

</style>