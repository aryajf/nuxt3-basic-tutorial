<template>
    <div>
        <h2>About</h2>
        <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Nulla aliquid eveniet assumenda repellat qui consectetur animi, magnam, et voluptas ipsa tempora. Voluptatibus officia saepe nam dolor consectetur doloremque voluptas temporibus.</p>
        <div>{{data}}</div>
    </div>
</template>

<script setup>
const {data} = await useFetch('/api?name=mario', {
    method: 'post',
    body: {age:30}
})
</script>

<style lang="scss" scoped>
    h2{
        margin-bottom: 20px;
        font-size:36px;
    }

    p{
        margin: 20px 0;
    }
</style>