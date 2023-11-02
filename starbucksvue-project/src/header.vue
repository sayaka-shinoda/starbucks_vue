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
    <div class="header_menu">
    <!-- Logo,MENU,REWARDS,GIFT CARDS -->
        <a href="https://www.starbucks.com/"><img src="@/assets/logo.png" alt="Logo" class="header_logo"></a>
    <!-- pc menu -->
    <div class="pc_menu">
        <ul class="menu_ul">
            <li class="header-left"><a href="https://www.starbucks.com/menu">{{ header_menu }}</a></li>
            <li class="header-left"><a href="https://www.starbucks.com/rewards">{{ header_rewards }}</a></li>
            <li class="header-left"><a href="https://www.starbucks.com/gift">{{ header_giftcards }}</a></li>
    <!-- Find a store,Sign in,join now -->
            <li class="header-right"><a href="https://www.starbucks.com/store-locator?map=39.635307,-101.337891,5z"><img src="@/assets/map_icon.svg" alt="map" class="map_icon">{{ header_findastore }}</a></li>
            <li class="header-right"><a href="https://www.starbucks.com/account/signin?ReturnUrl=%2F"><div class="signin_btn">{{ header_signin }}</div></a></li>
            <li class="header-right"><a href="https://www.starbucks.com/account/create"><div class="joinnow_btn">{{ header_joinnow }}</div></a></li>
        </ul>
    </div>
    <!-- mobile menu-->
    <div class="mobile_menu">
        <input type="checkbox" id="mobilemenu_check">
        <label for="mobilemenu_check" class="mobilemenu_box">
            <span></span>
        </label>
    <div class="mobilemenu_content">
        <ul class="mobilemenu_list">
        <li class="mobilemenu_item">
            <a class="mobilemenu__link" href="https://www.starbucks.com/menu"><div class="header_leftItem">{{ header_menu }}</div></a>
        </li>
        <li class="mobilemenu_item">
            <a class="mobilemenu__link" href="https://www.starbucks.com/rewards"><div class="header_leftItem">{{ header_rewards }}</div></a>
        </li>
        <li class="mobilemenu_item">
            <a class="mobilemenu__link" href="https://www.starbucks.com/gift"><div class="header_leftItem">{{ header_giftcards }}</div></a>
        </li>
        <li class="mobilemenu_item">
            <a class="mobilemenu__link" href="https://www.starbucks.com/store-locator" ><div class="header_leftItem">{{ header_findastore }}</div></a>
        </li>  
        <li class="mobilemenu_item">
            <a class="mobilemenu__link" href="https://www.starbucks.com/account/signin?ReturnUrl=%2F"><div class="header_leftItem signin_mobile_btn">{{ header_signin }}</div></a>
        </li>
        <li class="mobilemenu_item">
            <a class="mobilemenu__link" href="https://www.starbucks.com/account/create"><div class="header_leftItem joinnow_mobile_btn">{{ header_joinnow }}</div></a>    
        </li>
        </ul>
    </div>
    </div>
    </div>
</template>

<style scoped>
*{
    font-family: SoDoSans;
    font-weight: bold;
}
a{
    color: #212121;
}
.header_menu{
    width: 100%;
}
.header_menu a:hover{
    color: rgb(0 117 74);
}
.signin_btn,.signin_mobile_btn{
    color: black;
    border: 1px solid black;
    border-radius: 100px;
    display: block;
    width: 80px;
    padding: 2px;
    box-sizing: border-box;
    background-color: white;
    text-align: center;
}
.signin_btn:hover,.signin_mobile_btn:hover{
    background-color: gainsboro;
}
.joinnow_btn,.joinnow_mobile_btn{
    border: 1px solid black;
    border-radius: 100px;
    display: block;
    width: 80px;
    padding: 2px;
    box-sizing: border-box;
    color: white;
    background-color: black;
    text-align: center;
}
.joinnow_btn:hover,.joinnow_mobile_btn:hover{
    background-color: #404040;
}
.map_icon{
    width: 20px;
    height: 20px;
    margin: 0 10px;
}
.map_icon:hover{
    color: rgb(0 117 74)
}
/* mobile */
@media screen and (max-width:375px){
/* pc menu off */
    .pc_menu{
        display: none;
    }
    .mobilemenu_box {
        position: fixed;
        top: 0;
        right: 0;
        display: flex;
        height: 60px;
        width: 60px;
        justify-content: center;
        align-items: center;
        z-index: 90;
        background: transparent;
    }
    /* theree line button */
    .mobilemenu_box span,
    .mobilemenu_box span:before,
    .mobilemenu_box span:after {
        content: "";
        display: block;
        height: 3px;
        width: 25px;
        border-radius: 3px;
        background: black;
        position: absolute;
    }
    .mobilemenu_box span:before {
        bottom: 8px;
    }
    .mobilemenu_box span:after {
        top: 8px;
    }
    #mobilemenu_check {
        display: none;
    }
    #mobilemenu_check:checked ~ .mobilemenu_box span {
        background: rgba(255, 255, 255, 0);
    }
    #mobilemenu_check:checked ~ .mobilemenu_box span::before {
        bottom: 0;
        transform: rotate(45deg);
    }
    #mobilemenu_check:checked ~ .mobilemenu_box span::after{
        top: 0;
        transform: rotate(-45deg);
    }
    #mobilemenu_check:checked ~ .mobilemenu_content{
        left: 0;
    }
    .mobilemenu_content{
        width: 50%;
        height: 100%;
        position: fixed;
        top: 0;
        left: 100%;
        z-index: 80;
        background-color: white;
        transition: all 0.5s;
    }
    .mobilemenu_list{
        padding: 70px 10px 0;
    }
    .mobilemenu_item{
        border-bottom: solid 1px #ffffff;
        list-style: none;
    }
    .mobilemenu_link {
        display: block;
        width: 100%;
        font-size: 15px;
        box-sizing: border-box;
        color: #ffffff;
        text-decoration: none;
        padding: 9px 15px 10px 0;
    }
}
/* pc */
@media screen and (min-width:376px){
/* mobile menu off */
    .mobile_menu{
        display: none;
    }
    .header_menu{
        width: 100%;
        margin: 30px 0;
        display: flex;
    }
    .pc_menu {
        width: 100%;
        margin: 20px;
    }
    .pc_menu > ul {
        display: flex;
        list-style: none;
    }
    .pc_menu > ul > li {
        text-align: left;
        width: auto;
        margin: 0 15px;
    }
    .menu_ul>li:nth-of-type(3){
        margin-right: auto;
    }
}

</style>