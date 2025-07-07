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
    height: 35rem;
    background: url(./assets/img/header.jpg) no-repeat;
    background-size: 100% auto;
}
.rules{
    height: 21.3rem;
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
    height: 40rem;
    background: red;
   
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
