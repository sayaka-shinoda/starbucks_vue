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
        <input id="mobilemenu_Checkbox" type="checkbox" class="mobilemenu_input">
        <label for="mobilemenu_Checkbox" class="hamburgermenu_btn">
            <span class="hamburgermenu_line"></span>
        </label>
        <label for="mobilemenu_Checkbox" class="mobilemenu-background"></label>
    <div class="mobilemenu_content">
    <!-- MENU,REWARDS,GIFT CARDS -->
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
        </ul>
    <!-- line -->
        <hr>
    <!-- Sign in,Join now -->
        <div class="mobilemenu_btn">
            <a href="https://www.starbucks.com/account/signin?ReturnUrl=%2F"><div class="signin_mobile_btn">{{ header_signin }}</div></a>
            <a href="https://www.starbucks.com/account/create"><div class="joinnow_mobile_btn">{{ header_joinnow }}</div></a>   
        </div>
    <!-- Find a store -->
            <a class="find_a_store" href="https://www.starbucks.com/store-locator" ><img src="@/assets/map_icon.svg" alt="map" class="map_icon">{{ header_findastore }}</a>
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
    width: 95px;
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
    *{
        font-size: large;
    }
    /* hamburger menu button */
    .hamburgermenu_btn {
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
    .hamburgermenu_btn span,
    .hamburgermenu_btn span:before,
    .hamburgermenu_btn span:after {
        content: "";
        display: block;
        width: 25px;
        height: 3px;
        border-radius: 3px;
        background: black;
        position: absolute;
        transition: .3s;
    }
    .hamburgermenu_btn span:before {
        bottom: 8px;
    }
    .hamburgermenu_btn span:after {
        top: 8px;
    }
    #mobilemenu_Checkbox {
        display: none;
    }
    #mobilemenu_Checkbox:checked ~ .hamburgermenu_btn span {
        background: rgba(255, 255, 255, 0);
    }
    #mobilemenu_Checkbox:checked ~ .hamburgermenu_btn span::before {
        bottom: 0;
        transform: rotate(45deg);
    }
    #mobilemenu_Checkbox:checked ~ .hamburgermenu_btn span::after{
        top: 0;
        transform: rotate(-45deg);
    }
    /* menu slide */
    #mobilemenu_Checkbox:checked ~ .mobilemenu_content{
        left: 30%;
    }
    /* menu area */
    .mobilemenu_content{
        width: 70%;
        height: 100%;
        position: fixed;
        top: 0;
        left: 100%;
        z-index: 80;
        padding: 5em 3% 2em;
        background-color: white;
        transition: all 0.5s;
    }
    .mobilemenu_list{
        padding: 70px 10px 0;
    }
    /* menu open => background */
    .mobilemenu-background{
    display: none;
    position: fixed;
    z-index: 10;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background: #000;
    opacity: 0;
    transition: all 0.5s ease-in-out 0s;        
    }
    .mobilemenu_input:checked ~ .mobilemenu-background{
    display: block;
    opacity: 0.3;
    }
    /* MENU,REWARDS,GIFT CARDS */
    .mobilemenu_item{
        margin: 50px 15px;
        list-style: none;
    }
    /* Sign in,Join now */
    .mobilemenu_btn{
        display: flex;
    }
    .signin_mobile_btn{
        margin: 50px 0 50px 15px;
    }
    .joinnow_mobile_btn{
        margin: 50px 30px;
    }
    /* Find a Store */
    .find_a_store{
        margin-left: 15px;
    }
    /* line */
    hr{
        margin: 30px auto;
        width: 75%;
        height: 3px;
        border: none;
        background-color: rgb(214, 214, 214);
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