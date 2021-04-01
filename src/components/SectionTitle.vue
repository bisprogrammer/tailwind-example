<template>
    <h2 class="flex items-center justify-center">
        <span class="rhombus"></span>
        <span class="mx-4 text-4xl font-bold">{{title}}</span>
        <span class="rhombus"></span>
    </h2>
</template>

<script>

export default {
    props: ['title']
}
</script>

<style scoped>
.rhombus {
    width: 6.58px;
    height: 6.58px;
    background: #FE5F5F;
    transform: matrix(0.71, -0.64, 0.78, 0.71, 0, 0);
}
</style>
