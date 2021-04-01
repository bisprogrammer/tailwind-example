<template>
    <section class="max-w-screen-lg mx-auto mb-16 md:mb-32 lg:mb-64 px-4">
        <SectionTitle title="Преимущества" class="mb-6 md:mb-12 lg:mb-24" />
        <div class="flex flex-col md:flex-row">
            <div class="md:w-72 text-center flex flex-col"
                 :class="{ 'md:mr-12 lg:mr-24 mb-10 md:mb-0':  index !== 2}"
                 v-for="(item, index) in items"
                 :key="item.id">
                <img class="mb-4 h-48" :src="item.image" :alt="'advantage' + item.id">
                <span class="text-3xl md:text-5xl font-bold text-indigo-1000 mb-2 mt-auto">{{item.count}}</span>
                <p class="lg:text-xl font-bold">{{item.text}}</p>
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
