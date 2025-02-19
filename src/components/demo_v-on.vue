<!-- 一般简写为：@事件名="事件处理函数"
事件绑定指令 -->
<template>
<button @click="out">输出信息</button>
</template>
<script setup>
const out = ()=>{
    console.log('xixihaha')
}
</script>