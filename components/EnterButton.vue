<template>
    <div class='' @click='click'>
    <input type='button'/>
    </div>
    
</template>

<script>
import{mapGetters, mapMutations} from 'vuex'

export default{
    computed:{
        ...mapGetters({
            entered:'entered'
        })
    },
    methods:{
        enter(el,done){
            TweenMax.to(el,1.5,{
                opacity:1,
                x:0,
                startAt:{
                    opacity:0,
                    x:'-20px'
                },
                ease:Expo.easeOut,
                onComplete:()=>{
                    done()
                }
            })
        },
        leave(el,done){
            TweenMax.to(el,1.5,{
                opacity:0,
                x:'20px',
                startAt:{
                    opacity:1,
                    x:0
                },
                ease: Expo.easeOut,
                onComplete:()=>{
                    done()
                }
            })
        },
        ...mapMutations({
            click:'cilck'
        })
    }
}
</script>

<style lang='scss' scoped>
.TheButton{
    display: flex;
    justify-content:left;
    position: relative;
    width:100%;
    height:40px;

    &_Start{
        position:relative;
        margin:0;
        width:10rem;
        height:100%;
        cursor:pointer;
    }

    &_StartUnderline{
        position:absolute;
        bottom:0;
        width:100%;
        height:2px;
        background:#555;
    }
}
</style>