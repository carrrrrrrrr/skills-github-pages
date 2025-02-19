<template>
    <!-- 属性绑定指令 -->
    <div>
        <!-- 使用 :placeholder 绑定占位文本 -->
         <!--一般使用:属性名="数据名"-->
        <p><input type="text" :placeholder="username"></p>
        <p><input type="password" v-bind:placeholder="password"></p>
    </div>
</template>
<script setup>
import { ref } from 'vue';
const username = ref('请输入用户名');
const password = ref('请输入密码');
</script>