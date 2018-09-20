<template>
    <div class="header">
        <div class="header-left">
            <div class="iconfont backicon">&#xe639;</div>
        </div>
        <div class="header-input">
            <span class="iconfont">&#xe632;</span>
            输入城市游玩景点/主题
        </div>
        <router-link to="/city">
            <div class="header-right">{{this.doubleCity}}
                <span class="iconfont arrowicon">&#xe74d;</span>            
            </div>
        </router-link>
    </div>
</template>

<script>
import { mapState, mapGetters } from 'vuex'
export default {
    name: 'HomeHeader',
    computed: {
        ...mapState(['city']),
        ...mapGetters(['doubleCity'])
    }
}
</script>

<style lang="stylus" scoped>
    @import '~styles/variables.styl';
    .header
        display flex
        line-height $headerHeight
        background $bgColor
        color #fff
        .header-left
            width .64rem
            float left
            .backicon
                text-align center
                font-size .4rem
        .header-input
            flex 1
            height .64rem
            line-height .64rem
            margin-top .12rem
            margin-left .2rem
            padding-left .2rem
            background #ffffff
            border-radius .1rem
            color #ccc
        .header-right
            min-width 1.24rem
            float right
            text-align center
            color #fff
            .arrowicon
                margin-top -.02rem
                margin-left -.06rem
                font-size .34rem
</style>
