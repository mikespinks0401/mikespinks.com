<script lang="ts" setup>
    import { ref } from 'vue'
    import 'dotenv'

    const owner = ref('Michael Spinks')
    const test = ref("BLUE")
    const name = process.env.OWNER

</script>

<template>
    <div>
        <h1>About Me</h1>
        <h2 class="text-3xl text-green-400">{{owner}}</h2>
        <h3 class="font-black text-5xls">name = {{name}}</h3>
        <input class="px-4 py-2 bg-black text-white" v-model="test" />
    </div>
</template>