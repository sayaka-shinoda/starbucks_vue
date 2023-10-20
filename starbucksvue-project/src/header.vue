<script setup>
    import{ ref } from 'vue'
    const header_menu = ref('MENU')
    const header_rewards = ref('REWARDS')
    const header_giftcards = ref('GIFT CARDS')
    const header_findastore = ref('Find a store')
    const header_signin = ref('Sign in')
    const header_joinnow = ref('Join now')
</script>

<template>
    <div class="header">
    <!-- Logo,MENU,REWARDS,GIFT CARDS -->
    <div class="header-left">
        <a href="https://www.starbucks.com/"><img src="@/assets/logo.png" alt="Logo" class="header_logo"></a>
        <a href="https://www.starbucks.com/menu">
        <div class="header_leftItem">{{ header_menu }}</div></a>
        <a href="https://www.starbucks.com/rewards">
        <div class="header_leftItem">{{ header_rewards }}</div></a>
        <a href="https://www.starbucks.com/gift">
        <div class="header_leftItem">{{ header_giftcards }}</div></a>
        </div>
    <!-- Find a store,Sign in,join now -->
    <div class="header-right">
        <a href="https://www.starbucks.com/store-locator?map=39.635307,-101.337891,5z">
        <div class="header_rightItem">{{ header_findastore }}</div></a>
        <a href="https://www.starbucks.com/account/signin?ReturnUrl=%2F">
        <div class="header_rightItem signin_btn">{{ header_signin }}</div></a>
        <a href="https://www.starbucks.com/account/create">
        <div class="header_rightItem joinnow_btn">{{ header_joinnow }}</div></a>
        </div>
    </div>
</template>

<style>
a{
    color: #212121;
}
a:hover{
    color: #00754A;
    background-color: transparent;
}    
.header{
    width: 100%;
    margin: 50px 50px;
}
.header-right{
    display: flex;
    float: right;
}
.header-left{
    display: flex;
}
.header_leftItem,.header_rightItem{
    margin: 10px 20px;
    font-family: SoDoSans;
    font-weight: bold;
}
.signin_btn{
    border: 1px solid black;
    border-radius: 100px;
    display: block;
    width: 80px;
    padding: 2px;
    box-sizing: border-box;
    background-color: white;
    text-align: center;
    margin: 10px 0;
}
.signin_btn:hover{
    background-color: gainsboro;
}
.joinnow_btn{
    border: 1px solid black;
    border-radius: 100px;
    display: block;
    width: 80px;
    padding: 2px;
    box-sizing: border-box;
    color: white;
    background-color: black;
    text-align: center;
    margin: 10px 10px;
}
.joinnow_btn:hover{
    background-color: #404040;
}
</style>