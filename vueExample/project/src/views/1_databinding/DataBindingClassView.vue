<template>
  <div>
    <!-- 클래스명이 있으면 클래스가 적용 그렇지 않으면 적용이 안됨 -->
    <div :class="{'text-red': hasError, 'active': isActive}">클래스 바인딩</div>
    <div :class="class2">클래스 바인딩2</div>
  </div>
</template>

<script>
export default {
    data() {
        return {
            // css를 적용시킬 수 있는 변수들
            isActive: false,
            hasError: false,
            class2: ['active','hasError']
        }
    }
}
</script>

<style>
.active{
    background-color: greenyellow;
    font-weight: bold;
}

.text-red{
    color: red
}
</style>