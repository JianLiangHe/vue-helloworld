<template>
    <div class="first-app">
        {{msg}}
        <confirm text="注册" @message="getMessage"></confirm>
        <p>
            <router-link to="/second">跳到第二个页面</router-link>
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