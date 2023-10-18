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
    const birthday = ref('We’re celebrating PSL’s birthday. \n Yours is next!')
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
    <div class="content">
    <!-- HBD PSL -->
    <div class="first_content">
    <div class="mainimgA"><img src="@/assets/mainA.jpg" alt="content" class="first_content_img"></div>
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
    <div class="mainimgB"><img src="@/assets/mainB.jpg" alt="content" class="second_content_img"></div>
    </div>
    <!-- We’re celebrating PSL’s birthday.Yours is next! -->
    <div class="third_content">
    <div class="mainimgC"><img src="@/assets/mainC.jpg" alt="content" class="third_content_img"></div>    
    <div class="third_content_text">
        <h1><font color="white">{{ birthday }}</font></h1>
        <p><font color="white">{{ birthday_text }}</font></p>
        <p class="birthday_btn">{{ birthday_button  }}</p>
    </div>
    </div>
    <!-- Twice the spice -->
    <div class="fourth_content">
    <div class="fourth_content_text">
        <h1>{{ spice }}</h1>
        <p>{{ spice_text }}</p>
        <a class="spice_btn" href="https://www.starbucks.com/menu/product/2123236/single">{{ spice_button }}</a>
    </div>   
    <div class="mainimgD"><img src="@/assets/mainD.jpg" alt="content" class="fourth_content_img"></div> 
    </div>
    <!-- Pumpkin spice, delivered so nice -->
    <div class="fifth_content">
    <div class="mainimgE"><img src="@/assets/mainE.jpg" alt="content" class="fifth_content_img"></div> 
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

<style>
    .content{
        width: 1920px;
        height: 2600px;
    }
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
        height: 530px;
        text-align: center;
        background-color: #006241;
    }
    .second_content_text{
        width: 600px;
        height: 530px;
        text-align: center;
        background-color: rgb(176 74 90);
    }
    .third_content_text{
        width: 600px;
        height: 530px;
        text-align: center;
        background-color: #006241;
    }
    .fourth_content_text{
        width: 600px;
        height: 530px;
        text-align: center;
        background-color: rgb(214 154 45);
    }
    .third_content_text{
        width: 600px;
        height: 250px;
        text-align: center;
        background-color: rgb(30 57 50);
    }
    .fifth_content_text{
        width: 600px;
        height: 360px;
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
        margin: 100px 210px;
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
        margin: 100px 230px;
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
        margin: 100px 230px;
    }
    .spice_btn:hover{
        color: black;
        background-color: hsl(39, 67%, 43%);
    }
    .delivered_btn{
        border: 1px solid white;
        border-radius: 100px;
        display: block;
        width: 130px;
        padding: 5px;
        box-sizing: border-box;
        color: white;
        background-color: rgb(30 57 50);
        text-align: center;
        margin: 100px 230px;
    }
    .delivered_btn:hover{
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
        margin: 40px 10px;
    }
    p{
        margin: 50px 10px;
    }
</style>