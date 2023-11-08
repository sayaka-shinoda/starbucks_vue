<script setup>
    import{ ref } from 'vue'
    // HBD PSL
    const hbd_psl = ref('HBD PSL')
    const hbd_text = ref('Cheers for the drink that’s made fall “fall” for \n two decades.')
    const hbd_button = ref('Join the celebration')
    // Pumpkin forever
    const pumpkin_forever = ref('Pumpkin forever')
    const pumpkin_text = ref('Let the nostalgia begin. Enjoy a steamy \n creamy Pumpkin Spice Latte topped with \n pumpkin-pie spices.')
    const pumpkin_button = ref('Order now')
    // We’re celebrating PSL’s birthday.Yours is next!
    const birthday = ref('We’re celebrating PSL’s birthday.Yours is \n next!')
    const birthday_text = ref('Join Starbucks® Rewards and enjoy a free drink on your \n birthday every year.*')
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
    <!-- first line -->
    <hr>
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
    *{
        font-family: SoDoSans;
    }
    /* first line */
    hr{
        margin: 50px 0;
        width: 100%;
        height: 3px;
        border: none;
        background-color: rgb(214, 214, 214);
    }
    .first_content,.second_content,.third_content,.fourth_content,.fifth_content{
        display: flex;
        width: 100%;
        height: auto;
        margin: 30px 0;
        justify-content: center;
    }
    .first_content_img,.third_content_img,.fifth_content_img{
        width: 50%;
        height: auto;
    }
    .second_content_img,.fourth_content_img{
        width: 50%;
        height: auto;
    }
    .first_content_text{
        width: 50%;
        height: auto;
        text-align: center;
        background-color: #006241;
    }
    .second_content_text{
        width: 50%;
        height: auto;
        text-align: center;
        background-color: rgb(176 74 90);
    }
    .third_content_text{
        width: 50%;
        height: auto;
        text-align: center;
        background-color: rgb(30 57 50);
    }
    .fourth_content_text{
        width: 50%;
        height: auto;
        text-align: center;
        background-color: rgb(214 154 45);
    }
    .fifth_content_text{
        width: 50%;
        height: auto;
        text-align: center;
        background-color: rgb(30 57 50);
    }
    /* button */
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
        margin: auto;
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
        margin: auto;
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
        margin: auto;
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
        margin: auto;
    }
    .birthday_btn:hover,.delivered_btn:hover{
        color: white;
        background-color: rgb(24 46 40);
    }
    .Benefits-text{
        font-size: medium;
        margin: 50px auto;
        text-align: center;
    }
    div{
        white-space: pre-line;
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
    .third_content_text{
        height: 350px;
    }
    .fifth_content_text{
        height: 450px;
    }
    /* font */
    /* first,second,fourth */
    .first_content_text h1,
    .second_content_text h1,
    .fourth_content_text h1{
        font-size: 60px;
        margin-top: 10%;
    }
    .first_content_text p,
    .second_content_text p,
    .fourth_content_text p{
        font-size: 30px;
        margin: 30px;
        margin-bottom: 50px;
    }
    /* third */
    .third_content_text h1{
        font-size: 35px;
        margin-top: 5%;
    }
    .third_content_text p{
        font-size: 20px;
        margin: 15px;
        margin-bottom: 30px;
    }
    /* fifth */ 
    .fifth_content_text h1{
        font-size: 50px;
        margin-top: 10%;
    }
    .fifth_content_text p{
        font-size: 30px;
        margin: 30px;
        margin-bottom: 35px;
    }
    }
    /* pc */
    @media screen and (min-width:375px) {
/* font */
    /* first,second,fourth */
    .first_content_text h1,
    .second_content_text h1,
    .fourth_content_text h1{
        font-size: 45px;
        margin-top: 15%;
    }
    .first_content_text p,
    .second_content_text p,
    .fourth_content_text p{
        font-size: large;
        margin: 30px;
    }
    /* third */
    .third_content_text h1{
        font-size: 23px;
        margin-top: 2%;
    }
    .third_content_text p{
        font-size: medium;
        margin: 10px;
    }
    /* fifth */ 
    .fifth_content_text h1{
        font-size: 25px;
        margin-top: 15%;
    }
    .fifth_content_text p{
        font-size: medium;
        margin: 30px;
    }
    }
</style>