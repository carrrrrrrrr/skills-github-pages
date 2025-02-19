//reactive函数的学习与使用
//reactive函数的作用是创建一个响应式对象或数组，将普通的对象或数组转换为响应式对象或数组
<template>{{ object.message }}</template>
<script setup>
import { reactive } from 'vue'
const object = reactive({message: '嘻嘻'})
//响应式对象或数组 = reactive（对象或数组）
setTimeout(()=>{
    object.message = '呵呵'
},1000)
</script>