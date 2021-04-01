<template>
    <section class="bg-gray-1000 pt-16 pb-12 px-4 rounded-t-half">
        <div class="mx-auto w-72">
            <h2 class="text-2xl md:text-4xl font-bold mb-2">Есть вопросы?</h2>
            <p class="mb-7">Задайте интересующие вас вопросы онлайн помощнику</p>
            <Button class="bg-red-1000 px-12 mx-auto" label="Онлайн помощник">
                <img slot="before-label" class="mr-4" src="/img/helper.svg" alt="helper">
            </Button>
        </div>
    </section>
</template>

<script>
import Button from "../components/Button";

export default {
    components: {
        Button
    }
}
</script>