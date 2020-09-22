<template>
    <div>
        {{ $route.params }}
        {{ createdParams }}
        {{ mountedParams }}
        {{ beforeUpdateParams }}
    </div>
</template>


<script>
export default {
    data() { return {
        createdParams: {},
        mountedParams: {},
        beforeUpdateParams: {},
    }},
    created() {
        this.createdParams = this.$route.params
    },
    mounted() {
        this.mountedParams = this.$route.params
    },
    beforeUpdate() {
        this.beforeUpdateParams = this.$route.params
    }

}
</script>