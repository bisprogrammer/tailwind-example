<template>
    <section class="max-w-screen-lg mx-auto mb-6 sm:mb-12 md:mb-24 lg:mb-44 px-4">
        <SectionTitle title="Истории успеха" class="mb-6 md:mb-12" />
        <div>
            <div class="flex flex-col sm:flex-row sm:justify-between sm:text-left"
                :class="{ 'mb-6 lg:mb-12': index !==2 }"
                v-for="(item, index) in items"
                :key="item.id">
                <div class="w-64 sm:w-2/5 mx-auto"
                     :class="{ 'sm:order-1 sm:text-right': (index + 1) % 2 === 0 }">
                    <img class="inline" :src="item.avatar" alt="">
                </div>
                <div class="flex flex-col justify-center items-center sm:items-baseline sm:w-3/5 -mt-10 sm:mt-0 py-6 sm:py-12">
                    <h2 class="text-xl sm:text-2xl font-bold mb-5">{{item.title}}</h2>
                    <blockquote class="flex mb-4">
                        <img class="mr-3" src="/img/arrow_right.svg" alt="arrow_right">
                        <span class="text-red-1000 font-bold leading-5">{{item.blockquote}}</span>
                    </blockquote>
                    <p v-if="item.text" class="mb-3 leading-5">{{item.text}}</p>
                    <Button class="bg-indigo-1000 px-5 sm:mr-auto" :class="{ 'mt-auto': !item.text }" label="Читать историю">
                        <img slot="after-label" class="ml-3" src="/img/arrow_right_thin.svg" />
                    </Button>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
import SectionTitle from "../components/SectionTitle";
import Button from "../components/Button";

export default {
    props: ['items'],
    components: {
        SectionTitle,
        Button
    }
}
</script>