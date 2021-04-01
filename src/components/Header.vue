<template>
    <header class="mt-4 mb-16 max-w-screen-xl mx-auto">
        <div class="flex items-center justify-between mb-16">
            <div class="flex items-center">
                <Button class="bg-red-1000 mr-7 px-7" label="Личный кабинет" />
                <a href="#" class="text-blac font-bold">Каталог услуг</a>
            </div>
            <div class="flex items-center">
                <span class="flex justify-center items-center bg-red-1000 rounded-full mr-3 w-9 h-9">
                    <img src="/img/helper.svg" alt="">
                </span>
                <a href="#" class="text-red-1000 font-bold">Онлайн помощник</a>
            </div>
        </div>
        <div>
            <img src="img/logo.svg" alt="">
        </div>
    </header>
</template>

<script>
import Button from "../components/Button";

export default {
    components: {
        Button
    }
}
</script>