<template>
  <div>
    <select name="" id="" v-model="selectedCity">
        <option value=""></option>
        <option value="02">seoul</option>
        <option value="051">busan</option>
        <option value="064">jeju</option>
    </select>
  </div>
</template>

<script>
export default {
    data() {
        return {
            selectedCity: '02'
        }
    }
}
</script>

<style>

</style>