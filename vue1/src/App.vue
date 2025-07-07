<template>
    <div>
        <div class="head">

        </div>
        <div class="rules">
            <img src="./assets/img/button_rewards.png" alt="" class="png1">
            <span class="png2">Rules</span>
            <div class="time">
                <b>10</b>
                <b class="lf">D</b>
                <b class="rg">12</b>
                <span>:</span>
                <b>21</b>
                <span>:</span>
                <b>09</b>
            </div>
            <div class="wenzi">
                Oyelite brings an amazing event!
                When you recharge through PhonePe UPI,
                you can get an extra reward for every single recharge!
            </div>
        </div>
        <div class="bangdan">
            <div class="bangdan1">
                <span class="bangdan-lf">Recharge Amount</span>
                <span class="bangdan-rg">Rewards</span>
                <div class="bangdan2">
                    <div class="bangdan-img f1">1</div>
                    <div class="bangdan-img f2">2</div>
                    <div class="bangdan-img f2">3</div>
                    <div class="bangdan-img f2">4</div>
                    <div class="bangdan-img f2">5</div>
                </div>
                <div class="bangdan3">
                    1
                </div>
            </div>
        </div>
    </div>
</template>
<style lang="less">
*{
    padding: 0;
    margin: 0;
    color: white;
}
html,body{
    font-size: 12px;
}
.head{
    width: 100%;
    height: 32.55rem;
    background: url(./assets/img/header.jpg) no-repeat;
    background-size: 100% auto;
}
.rules{
    height: 18rem;
    width: 100%;
    background: url(./assets/img/bg_rewards.jpg) no-repeat;
    background-size: 100% auto;
    position: relative;
    .png1{
    width: 4.3rem;
    height: 4.3rem;
    position: absolute;

}
    .png2{
    width: 6.5rem;
    height: 3rem;
    background: url(./assets/img/button_rules.png) no-repeat;
    background-size: 100% auto;
    position: absolute;
    right: 0;
    display: flex;
    justify-content: center;
    align-items: center;
    font-size: 1.3rem;
}
    .time{
        position: absolute;
        left: 50%;
        transform: translateX(-50%);
        top: 0.9rem;
        display: flex;
        justify-content: center;
    }
    .time>b{
        width: 2.3rem;
        height: 2.3rem;
        border: .1rem solid #FFF665;
        box-sizing: border-box;
        display: block;
        line-height: 2.3rem;
        text-align: center;
        background: #AA212F;
        border-radius: 25%;
        font-size: 1.3rem;
    }
    .lf{
        margin-left: 0.3rem;
    }
    .rg{
        margin-left: 0.5rem;
    }
    .time>span{
        width: 0.5rem;
        height: 0.5rem;
        font-size: 1.3rem;
        text-align: center;
    }
    .wenzi{
        position: absolute;
        top: 5.5rem;
        left: 5rem;
        right: 10.5rem;
        font-size: 1.2rem;
    }
}
.bangdan{
    width: 100%;
    height: 44rem;
    background: url(./assets/img/border.png) no-repeat;
    background-size: 100% auto;
    z-index: auto;
    position: absolute;
    
    .bangdan1{
        width: 100%;
        height: 42rem;
        background: #A30007;
        position: relative;
        z-index: -1;
        margin-top: 1rem;
        box-sizing: border-box;
        top: .1rem;
    }
    .bangdan-lf{
        font-size: 1.3rem;
        color: #B14911;
        position: absolute;
        left: 5rem;
        top: 3rem;
    }
    .bangdan-rg{
        font-size: 1.3rem;
        color: #B14911;
        position: absolute;
        right: 5rem;
        top: 3rem;
    }
    .bangdan2{
        width: 100%;
        height: 30rem;
        position: absolute;
        left: 7.5%;
        top: 6rem;
    }
    .bangdan-img{
        width: 85%;
        height: 5rem;
        background: blue;
        
    }
    .f2{
        margin-top: 1.25rem;
    }
    .bangdan3{
        width: 85%;
        height: 3.5rem;
        background: pink;
        position: absolute;
        left: 7.5%;
        top: 37rem;
    }
}

</style>
<script setup>
    import { onMounted } from 'vue';
onMounted(()=>{
    let scaleW=window.innerWidth/375;
    let fontSize = 10 * scaleW;
    document.documentElement.style.fontSize = fontSize + 'px';
    window.addEventListener('resize',()=>{
    let scaleW = window.innerWidth / 375;
    let fontSize = 10 * scaleW;
    document.documentElement.style.fontSize = fontSize + 'px';
    })
})
</script>
