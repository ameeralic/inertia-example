<template>
    <h1>Hello {{ name }}</h1>
    <Link href="/home">home</Link>
    <h3 v-for="(item, index) in frameworks" :key="index">
        {{ item }}
    </h3>
</template>
<script>
import { Link } from '@inertiajs/vue3'
export default {
    props:['name','frameworks'],
    components:{
        Link
    }
}
</script>