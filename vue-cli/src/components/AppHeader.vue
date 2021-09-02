<template>
    <header>
        <h1>{{propsdata}}</h1>
        <button v-on:click="sendEvent">send</button>
    </header>
</template>

<script>
export default {
    props: ['propsdata'],
    methods : {
        sendEvent: function() {
            //상위 컴포넌트에 전달
            this.$emit('renew')
        }
    }
};
</script>
<style lang="scss" scoped>
</style>