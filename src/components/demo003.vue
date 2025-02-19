<template>
    {{ msg }}
</template>
<script setup>
let msg = '闪光魔法'
setTimeout(() => {
    console.log('使用闪光魔法之前'+msg);
    msg = '爆炸魔法'
    console.log('使用闪光魔法之后'+msg);
}, 500);
</script>