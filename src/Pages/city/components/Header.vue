<template>
    <div class="header">
        城市选择
        <router-link to="/">
            <div class="iconfont backicon">&#xe639;</div>
        </router-link>
    </div>
</template>

<script>
export default {
    name: "CityHeader"
}
</script>

<style lang="stylus" scoped>
    @import '~styles/variables.styl'
    .header
        overflow hidden
        position relative
        height $headerHeight
        line-height $headerHeight
        text-align center
        color #fff
        background $bgColor
        font-size .32rem
        .backicon
            width .64rem
            position absolute
            text-align center
            font-size .4rem
            top 0
            left 0
            color #fff
</style>
