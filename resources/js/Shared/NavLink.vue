<template>
    <Link :class="{'active': active }"><slot></slot></Link>
</template>
<script setup>
defineProps(['active'])
</script>
<style scoped>
.active {
    color:rgb(0, 42, 133);
    font-weight: bold;
}
</style>