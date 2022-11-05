<template>
  <div>
    <button @click="increseCounter">Add 1</button>
    <p>{{counter}}</p>
  </div>
</template>

<script>
export default {
    data() {
        return {
            counter: 0
        }
    },
    methods: {
        increseCounter() {
            this.counter += 1
        }
    }
}
</script>

<style>

</style>