<template>
    <button class="rounded-2xl text-white py-2 focus:outline-none flex justify-center items-center">
        <slot name="before-label"></slot>
        <span>{{label}}</span>
        <slot name="after-label"></slot>
    </button>
</template>

<script>

export default {
    props: ['label']
}
</script>