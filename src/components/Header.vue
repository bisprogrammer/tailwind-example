<template>
    <header class="max-w-screen-xl mt-4 mb-8 lg:mb-16 mx-auto px-4">
        <div class="flex items-center justify-between mb-8 lg:mb-16">
            <div class="flex items-center">
                <Button class="bg-red-1000 text-sm sm:text-base mr-3 sm:mr-7 px-3 sm:px-7" label="Личный кабинет" />
                <a href="#" class="text-sm sm:text-base font-bold">Каталог услуг</a>
            </div>
            <div class="flex items-center">
                <a href="#" class="text-red-1000 font-bold flex items-center">
                    <span class="flex justify-center items-center bg-red-1000 rounded-full mr-3 w-9 h-9">
                        <img src="/img/helper.svg" alt="">
                    </span>
                    <span class="hidden sm:inline">Онлайн помощник</span>
                </a>
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