<template>
    <div v-text="a"></div>
    <div v-html="a"></div>
</template>
<script setup>
const a = '<span>aaaaaaa</span>'
</script>