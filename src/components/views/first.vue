<template>
    <div class="first-app">
        {{msg}}
        <confirm text="注册" @message="getMessage"></confirm>
    </div>
</template>

<script>
import Confirm from '../sub/Confirm'
export default {
    name: 'first',
    data() {
        return {
            msg: 'welcome to first app'
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