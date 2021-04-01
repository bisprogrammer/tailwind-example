<template>
    <section class="max-w-screen-lg mx-auto mb-64">
        <SectionTitle title="Преимущества" class="mb-24" />
        <div class="flex">
            <div class="w-72 text-center flex flex-col"
                 :class="{ 'mr-24':  index !== 2}"
                 v-for="(item, index) in items"
                 :key="item.id">
                <img class="mb-4 h-48" :src="item.image" :alt="'advantage' + item.id">
                <span class="text-5xl font-bold text-indigo-1000 mb-2 mt-auto">{{item.count}}</span>
                <p class="text-xl font-bold">{{item.text}}</p>
            </div>
        </div>
    </section>
</template>

<script>
import SectionTitle from "../components/SectionTitle";

export default {
    props: ['items'],
    components: {
        SectionTitle
    }
}
</script>
