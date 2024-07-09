<template>
    <view>
        子组件单独引用 wd-toast（正常）
        <wd-button @click="test">测试(子组件)</wd-button>
        <wd-toast />
    </view>
</template>

<script setup>
import { useToast } from 'wot-design-uni';

const toast = useToast();

const test = () => {
    toast.warning('子组件单独引用 wd-toast（正常）');
};
</script>

<style scoped lang="scss"></style>
