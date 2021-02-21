<template>
    <div class="second-app">
        {{msg}}
        <p>
            <router-link to="/first">跳到第一个页面</router-link>
        </p>
    </div>
</template>

<script>
export default {
    name: 'Second',
    data() {
        return {
            msg: 'welcome to second app'
        };
    }
}
</script>