<script setup>
    import{ ref } from 'vue'
</script>

<template>
    <div class="main">
    <div class="contentA">
    <div class="mainimgA"><img src="@/assets/mainA.jpg" alt="content" class="main-imgA"></div>
    <div class="maintextA">
        <h1><font color="white">HBD PSL</font></h1>
        <p><font color="white">Cheers for the drink that’s made fall “fall” for<br>two decades.</font></p>
    </div>
    </div>
    <div class="contentB">
    <div class="maintextB">
        <h1><font color="white">Pumpkin forever</font></h1>
        <p><font color="white">Let the nostalgia begin. Enjoy a<br>steamy creamy Pumpkin Spice<br>Latte topped with pumpkin-pie<br>spices.</font></p>
    </div>
    <div class="mainimgB"><img src="@/assets/mainB.jpg" alt="content" class="main-imgB"></div>
    </div>
    <div class="contentC">
    <div class="mainimgC"><img src="@/assets/mainC.jpg" alt="content" class="main-imgC"></div>    
    <div class="maintextC">
        <h1><font color="white">We’re celebrating PSL’s birthday.<br>Yours is next!</font></h1>
        <p><font color="white">Join Starbucks® Rewards and enjoy a free<br>drink on your birthday every year.*</font></p>
    </div>
    </div>
    <div class="contentD">
    <div class="maintextD">
        <h1>Twice the<br>spice</h1>
        <p>Pair your PSL with its sidekick, the sweet and<br>salty Pumpkin Cream Cheese Muffin.</p>
    </div>   
    <div class="mainimgD"><img src="@/assets/mainD.jpg" alt="content" class="main-imgD"></div> 
    </div>
    <div class="contentE">
    <div class="mainimgE"><img src="@/assets/mainE.jpg" alt="content" class="main-imgE"></div> 
    <div class="maintextE">
        <h1><font color="white">Pumpkin spice, delivered so nice</font></h1>
        <p><font color="white">Your fall favorites, at your door— when you order<br>Starbucks delivery with DoorDash.**</font></p>
    </div>
    </div>
    <div class="maintextF">
        *At participating stores. To qualify for the Birthday Reward, you must have made at least<br>one Star-earning transaction prior to your birthday each year.
        <br><br><br>
        **See the DoorDash app for availability and restrictions. Menu limited.
    </div>
    </div>
</template>

<style>
    .main{
        width: 1920px;
        height: 2600px;
    }
    .contentA,.contentB,.contentC,.contentD,.contentE{
        display: flex;
        margin: 30px;
    }
    .main-imgA,.main-imgC,.main-imgE{
        width: 600px;
        height: 100%;
    }
    .main-imgB,.main-imgD{
        width: 600px;
        height: 100%;
    }
    .maintextA,.maintextC{
        width: 600px;
        height: 530px;
        text-align: center;
        background-color: #006241;
    }
    .maintextB{
        width: 600px;
        height: 530px;
        text-align: center;
        background-color: rgb(176 74 90);
    }
    .maintextD{
        width: 600px;
        height: 530px;
        text-align: center;
        background-color: rgb(214 154 45);
    }
    .maintextC{
        width: 600px;
        height: 250px;
        text-align: center;
        background-color: rgb(30 57 50);
    }
    .maintextE{
        width: 600px;
        height: 360px;
        text-align: center;
        background-color: rgb(30 57 50);
    }
    .maintextF{
        margin: 50px 350px;
        font-family: SoDoSans;
    }
    h1{
        margin: 40px 10px;
    }
    p{
        margin: 50px 10px;
    }
</style>