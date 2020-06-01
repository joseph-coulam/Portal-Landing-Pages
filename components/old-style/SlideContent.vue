<template>
    <div class="w-full mx-auto p-4">
        <div class="w-full shadow-lg text-gray-600 p-8 bg-white rounded-lg">
            <div class="text-sm pb-2 flex-grow">
                <h2 class="text-3xl text-black font-bold leading-tight mb-2">{{title}}</h2>
            </div>
            <ul class="font-display text-sm tracking-widest list-none uppercase">
                <li v-for="menuItem in list" :key="menuItem" class="mb-2">{{menuItem}}</li>
            </ul>
        </div>
    </div>
</template>

<script>
export default {
    props: {
        title: String,
        list: Array
    }
}
</script>