//ref函数的使用学习数据转换为响应式数据
<template>
<div>{{ message }}
</div>
</template>
<script setup>
import { ref } from 'vue'
const message = ref('嘻嘻')
setTimeout(() => {
    message.value = '呵呵'
}, 2000)
setTimeout(() => {
    message.value = '哈哈'
}, 3000)
setTimeout(() => {
    message.value = '嘿嘿'
}, 4000)
</script>