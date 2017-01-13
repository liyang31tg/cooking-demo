<template>
    <div>
        <h1>首页</h1>
        <p>A vue project. indexasdfjsasdfasdf2</p>
        <button @click="ccc">vvvvvvv</button>
        <button @click="showToast">showToastd</button>
        <mt-button type="primary" @click="showMsgbox">showMsgbox</mt-button>
        <mt-button type="primary" @click="sheetVisible = true">
            选择操作
        </mt-button>
    </div>
</template>
<script>
import {
    Toast,
    MessageBox
} from 'mint-ui';

export default {
    name: 'app',
    methods: {
        ccc: function() {
            console.log("cccccc")

        },
        showToast() {
            Toast('这是一个 Toast');
        },

        showMsgbox() {
            MessageBox('提示', '这是一个 Message Box');
        }

    }
};
</script>
<style>
html {
    text-align: center;
}
</style>
