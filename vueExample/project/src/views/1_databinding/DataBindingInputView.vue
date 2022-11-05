<template>
  <div>
    <input type="text" v-model="userId" />
    <button @click="clickBtn">클릭</button>
    <button @click="changeData">변경</button>
    <br>
    <input type="text" v-model="num1"/>+
    <input type="text" v-model="num2"/>=
    <span>{{num1 + num2}}</span>
    <br />
    <input type="text" v-model.number="num3"/>+
    <input type="text" v-model.number="num4"/>=
    <span>{{num3 + num4}}</span>
  </div>
</template>

<script>
export default {
    components: {},
    data() {
        return{
            userId: '자동바인딩',
            num1: 0,
            num2: 0,
            num3: 0,
            num4: 0,
        }
    },
    methods: {
        clickBtn(){
            alert(this.userId);
        },
        changeData() {
            this.userId = '새로운 값'
        }
    }
}
</script>

<style>

</style>