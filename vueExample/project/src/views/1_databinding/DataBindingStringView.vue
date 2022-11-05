<template>
    <div>
        <h1>Hello {{username}}</h1>
        <p>{{message}}</p>
    </div>
</template>
<script>
export default {
    data () {
        return {
            username: 'Park',
            message: 'Welcome dragon world',
            arr: [],
            obj: {}
        }
    }
}
</script>