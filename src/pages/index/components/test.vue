<template>
    <view>
        子组件不单独引用 wd-toast（无法使用）
        <wd-button @click="test">测试(子组件)</wd-button>
    </view>
</template>

<script setup>
import { useToast } from 'wot-design-uni';

const toast = useToast();

const test = () => {
    toast.warning('子组件不单独引用 wd-toast（无法使用）');
};
</script>

<style scoped lang="scss"></style>
