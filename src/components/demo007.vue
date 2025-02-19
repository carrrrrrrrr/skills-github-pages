<template>
    {{ message.value }}
    {{ object.message  }}
</template>
<script setup>
import { ref, reactive, toRefs } from 'vue'
const object = reactive({message: '嘻嘻'})
let {message} = toRefs(object)
//响应式对象或数组 = reactive（对象或数组）
setTimeout(()=>{
    message.value = '呵呵'
},1000)
</script>