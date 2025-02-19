//toref函数的学习与使用
//将响应式对象的单个属性转化为响应式数据(返回的是一个对象)
//响应式数据 = reactive(响应式对象，属性名)
<template>
    {{  message}}
    {{ object.message  }}
</template>
<script setup>
import { reactive, toRef } from 'vue'
const object = reactive({message: '嘻嘻'})
const message = toRef(object,'message')
setTimeout(()=>{
    message.value = '哈哈'
},2000)
</script>