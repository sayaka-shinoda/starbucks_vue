<script setup>
    import{ ref } from 'vue'
    // HBD PSL
    const hbd_psl = ref('HBD PSL')
    const hbd_text = ref('Cheers for the drink that’s made fall “fall” for \n two decades.')
    const hbd_button = ref('Join the celebration')
    // Pumpkin forever
    const pumpkin_forever = ref('Pumpkin forever')
    const pumpkin_text = ref('Let the nostalgia begin. Enjoy a \n steamy creamy Pumpkin Spice \n Latte topped with pumpkin-pie \n spices.')
    const pumpkin_button = ref('Order now')
    // We’re celebrating PSL’s birthday.Yours is next!
    const birthday = ref('We’re celebrating PSL’s birthday.Yours is \n next!')
    const birthday_text = ref('Join Starbucks® Rewards and enjoy a free \n drink on your birthday every year.*')
    const birthday_button = ref('Join now')
    // Twice the spice
    const spice = ref('Twice the \n spice')
    const spice_text = ref('Pair your PSL with its sidekick, the sweet and \n salty Pumpkin Cream Cheese Muffin.')
    const spice_button = ref('Order now')
    // Pumpkin spice, delivered so nice
    const delivered = ref('Pumpkin spice, delivered so nice')
    const delivered_text = ref('Your fall favorites, at your door— when you order \n Starbucks delivery with DoorDash.**')
    const delivered_button = ref('Order now')
    // Birthday Reward
    const birthday_reward = ('*At participating stores. To qualify for the Birthday Reward, you must have made at least \n one Star-earning transaction prior to your birthday each year. \n\n\n **See the DoorDash app for availability and restrictions. Menu limited.')
</script>

<template>
<head>
    <meta name="viewport" content="width=device-width">
</head>
    <div class="content">
    <!-- HBD PSL -->
    <div class="first_content">
    <img src="@/assets/hbd_psl.jpg" alt="content" class="first_content_img">
    <div class="first_content_text">
        <h1><font color="white">{{ hbd_psl }}</font></h1>
        <p><font color="white">{{ hbd_text }}</font></p>
        <a class="hbd_btn" href="https://www.starbucks.com/account/create">{{ hbd_button }}</a>
    </div>
    </div>
    <!-- Pumpkin forever -->
    <div class="second_content">
    <div class="second_content_text">
        <h1><font color="white">{{ pumpkin_forever }}</font></h1>
        <p><font color="white">{{ pumpkin_text }}</font></p>
        <a class="pumpkin_btn" href="https://www.starbucks.com/menu/product/2123774/iced">{{ pumpkin_button }}</a>
    </div>
    <img src="@/assets/pumpkin_forever.jpg" alt="content" class="second_content_img">
    </div>
    <!-- We’re celebrating PSL’s birthday.Yours is next! -->
    <div class="third_content">
    <img src="@/assets/birthday.jpg" alt="content" class="third_content_img">
    <div class="third_content_text">
        <h1><font color="white">{{ birthday }}</font></h1>
        <p><font color="white">{{ birthday_text }}</font></p>
        <a class="birthday_btn" href="https://www.starbucks.com/account/create">{{ birthday_button  }}</a>
    </div>
    </div>
    <!-- Twice the spice -->
    <div class="fourth_content">
    <div class="fourth_content_text">
        <h1>{{ spice }}</h1>
        <p>{{ spice_text }}</p>
        <a class="spice_btn" href="https://www.starbucks.com/menu/product/2123236/single">{{ spice_button }}</a>
    </div>   
    <img src="@/assets/spice.jpg" alt="content" class="fourth_content_img">
    </div>
    <!-- Pumpkin spice, delivered so nice -->
    <div class="fifth_content">
    <img src="@/assets/delivered.jpg" alt="content" class="fifth_content_img">
    <div class="fifth_content_text">
        <h1><font color="white">{{ delivered }}</font></h1>
        <p><font color="white">{{ delivered_text }}</font></p>
        <a class="delivered_btn" href="https://www.doordash.com/business/starbucks-1133/?ignore_splash_experience=true&utm_source=Enterprise&utm_medium=Enterprise&utm_campaign=CX_US_EP_EP_EP_PAR_CUSXXX__+Starbucks_Oct_Evergreen_Delivery_Landing_Page_Web">{{ delivered_button }}</a>
    </div>
    </div>
    <!-- Birthday Reward -->
    <div class="Benefits-text">{{ birthday_reward }}</div>
    </div>
</template>

<style scoped>
    .first_content,.second_content,.third_content,.fourth_content,.fifth_content{
        display: flex;
        margin: 30px;
    }
    .first_content_img,.third_content_img,.fifth_content_img{
        width: 600px;
        height: 100%;
    }
    .second_content_img,.fourth_content_img{
        width: 600px;
        height: 100%;
    }
    .first_content_text{
        width: 600px;
        height: 520px;
        padding: 100px;
        text-align: center;
        background-color: #006241;
    }
    .second_content_text{
        width: 600px;
        height: 520px;
        padding: 100px;
        text-align: center;
        background-color: rgb(176 74 90);
    }
    .third_content_text{
        width: 700px;
        height: 233px;
        text-align: center;
        background-color: rgb(30 57 50);
    }
    .third_content_text h1{
        font-size: 25px;
    }
    .fourth_content_text{
        width: 600px;
        height: 520px;
        padding: 100px;
        text-align: center;
        background-color: rgb(214 154 45);
    }
    .fifth_content_text{
        width: 600px;
        height: 350px;
        text-align: center;
        background-color: rgb(30 57 50);
    }
    .hbd_btn{
        border: 1px solid white;
        border-radius: 100px;
        display: block;
        width: 180px;
        padding: 5px;
        box-sizing: border-box;
        color: white;
        background-color: #006241;
        text-align: center;
        margin: 50px 110px;
}
.hbd_btn:hover{
        color: white;
        background-color: rgb(0 78 52);
}
    .pumpkin_btn{
        border: 1px solid white;
        border-radius: 100px;
        display: block;
        width: 130px;
        padding: 5px;
        box-sizing: border-box;
        color: white;
        background-color: rgb(176 74 90);
        text-align: center;
        margin: 50px 130px;
}
    .pumpkin_btn:hover{
        color: white;
        background-color: rgb(141 59 72);
    }
    .spice_btn{
        border: 1px solid black;
        border-radius: 100px;
        display: block;
        width: 130px;
        padding: 5px;
        box-sizing: border-box;
        color: black;
        background-color: rgb(214 154 45);
        text-align: center;
        margin: 50px 110px;
    }
    .spice_btn:hover{
        color: black;
        background-color: hsl(39, 67%, 43%);
    }
    .birthday_btn,.delivered_btn{
        border: 1px solid white;
        border-radius: 100px;
        display: block;
        width: 130px;
        padding: 5px;
        box-sizing: border-box;
        color: white;
        background-color: rgb(30 57 50);
        text-align: center;
        margin: 30px 230px;
    }
    .birthday_btn:hover,.delivered_btn:hover{
        color: white;
        background-color: rgb(24 46 40);
    }
    .Benefits-text{
        margin: 50px 350px;
        font-family: SoDoSans;
    }
    div{
        white-space: pre-line;
    }
    h1{
        font-family: SoDoSans;
        font-size: 45px;
    }
    p{
        margin: 20px 0;
    }
    /* mobile */
    @media screen and (max-width:375px){
    .first_content,.second_content,.third_content,.fourth_content,.fifth_content{
        flex-flow: column;
    }
    .second_content,.fourth_content{
        flex-direction: column-reverse;
    }
    .first_content_img,.second_content_img,.third_content_img,.fourth_content_img,.fifth_content_img{
        width: 100%;
    }
    .first_content_text,.second_content_text,.third_content_text,.fourth_content_text,.fifth_content_text{
        width: 100%;
    }
    .first_content_text,.second_content_text,.fourth_content_text{
        height: 600px;
    }
    .third_content_text,.fifth_content_text{
        height: 500px;
    }
    .hbd_btn,.pumpkin_btn,.birthday_btn,.spice_btn,.delivered_btn{
        margin: auto;
    }
    .Benefits-text{
        text-align: center;
        margin: auto;
    }
    }
    /* pc */
    @media screen and (min-width:1200px) {

    }
</style>