<template>
    <page>
        <view>
            <view class="item">
                page中引用了wd-toast（正常）
                <wd-button @click="test">测试</wd-button>
            </view>

            <TestCom class="item" />

            <TestCom2 class="item" />
        </view>
    </page>
</template>

<script setup>
import { useToast } from 'wot-design-uni';
import page from '../../components/page.vue';
import TestCom from './components/test.vue';
import TestCom2 from './components/test2.vue';

const toast = useToast();

const test = () => {
    toast.warning('page中引用了wd-toast（正常）');
};
</script>

<style scoped lang="scss">
.item {
    margin: 15px;
}
</style>
