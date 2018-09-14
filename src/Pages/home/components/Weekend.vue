<template>
<div>
    <div class="title">热销推荐</div>
    <ul>
        <li class="item border-bottom" v-for="item of recommendList" :key="item.id">
            <div class="item-img-wrapper">
                <img class="item-img" :src="item.imgUrl">                
            </div>
            <div class="item-info">
                <p class="item-title">{{item.title}}</p>
                <p class="item-desc">{{item.desc}}</p>
            </div>
        </li>
    </ul>
</div>
</template>

<script>
export default {
    name:'HomeWeekend',
    data () {
        return {
            recommendList: [{
                id: '0001',
                imgUrl: 'http://img1.qunarzz.com/sight/source/1505/3b/90c6e4c0a3d7bf.jpg_r_640x214_5f7b77f9.jpg',
                title: '常州中华恐龙园',
                desc: '以恐龙为主题的综合性游乐园'
            }, {
                id: '0002',
                imgUrl: 'http://img1.qunarzz.com/sight/source/1505/3b/90c6e4c0a3d7bf.jpg_r_640x214_5f7b77f9.jpg',
                title: '常州中华恐龙园',
                desc: '以恐龙为主题的综合性游乐园'
            }, {
                id: '0003',
                imgUrl: 'http://img1.qunarzz.com/sight/source/1505/3b/90c6e4c0a3d7bf.jpg_r_640x214_5f7b77f9.jpg',
                title: '常州中华恐龙园',
                desc: '以恐龙为主题的综合性游乐园'
            }, {
                id: '0004',
                imgUrl: 'http://img1.qunarzz.com/sight/source/1505/3b/90c6e4c0a3d7bf.jpg_r_640x214_5f7b77f9.jpg',
                title: '常州中华恐龙园',
                desc: '以恐龙为主题的综合性游乐园'
            }, {
                id: '0005',
                imgUrl: 'http://img1.qunarzz.com/sight/source/1505/3b/90c6e4c0a3d7bf.jpg_r_640x214_5f7b77f9.jpg',
                title: '常州中华恐龙园',
                desc: '以恐龙为主题的综合性游乐园'
            }, {
                id: '0006',
                imgUrl: 'http://img1.qunarzz.com/sight/source/1505/3b/90c6e4c0a3d7bf.jpg_r_640x214_5f7b77f9.jpg',
                title: '常州中华恐龙园',
                desc: '以恐龙为主题的综合性游乐园'
            }, {
                id: '0007',
                imgUrl: 'http://img1.qunarzz.com/sight/source/1505/3b/90c6e4c0a3d7bf.jpg_r_640x214_5f7b77f9.jpg',
                title: '常州中华恐龙园',
                desc: '以恐龙为主题的综合性游乐园'
            }]    
        }
    }
}
</script>

<style lang="stylus" scoped>
@import '~styles/mixins.styl'
    .title
        margin-top .2rem
        line-height .8rem
        background #eee
        text-indent .2rem
    .item
        .item-img-wrapper
            overflow hidden
            height 0
            padding-bottom 37%
            .item-img
                width 100%
        .item-info
            padding .1rem
            .item-title
                line-height .54rem
                font-size .32rem
                ellipsis()
            .item-desc
                line-height .4rem
                color #ccc
                ellipsis()            
</style>
