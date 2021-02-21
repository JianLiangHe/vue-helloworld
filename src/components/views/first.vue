<template>
    <div class="first-app">
        {{msg}}
        <confirm text="注册" @message="getMessage"></confirm>
        <p>
            <router-link to="/second">跳到第二个页面</router-link>
        </p>
        <p>
            <span class="blue-font">蓝色字体</span>
        </p>
    </div>
</template>

<script>
import Confirm from '../sub/Confirm'

export default {
    name: 'First',
    data() {
        return {
            msg: 'welcome to First app'
        };
    },
    components: {
        Confirm
    },
    methods: {
        getMessage(val) {
            alert(val);
        }
    }
}
</script>
<style lang="less">
.first-app {
    font-size: 30px;
    p {
        .blue-font {
            color: blue;
        }
    }
}
</style>