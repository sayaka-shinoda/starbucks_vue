<script setup>
    import{ ref } from 'vue' 
    // About Us
    const about_us = ref('About Us')
    const our_company = ref('Our Company')
    const our_coffee = ref('Our Coffee')
    const stories = ref('Stories and News')
    const starbucks_archive = ref('Starbucks Archive')
    const investor_relations = ref('Investor Relations')
    const customer_service = ref('Customer Service')
    const contact_us = ref('Contact Us')
    // Careers
    const careers = ref('Careers')
    const culture = ref('Culture and Values') 
    const inclusion = ref('Inclusion, Diversity, and \n Equity')
    const college = ref('College Achievement \n Plan')
    const alumni_community = ref('Alumni Community')
    const us_careers = ref('U.S. Careers')
    const international = ref('International Careers')
    // Social Impact
    const social_impact = ref('Social Impact')
    const people = ref('People')
    const planet = ref('Planet')
    const environmental = ref('Environmental and Social \n Impact Reporting')
    // For Business Partners
    const business_partners = ref('For Business Partners')
    const landlord = ref('Landlord Support Center')
    const suppliers = ref('Suppliers')
    const corporate = ref('Corporate Gift Card Sales')
    const office = ref('Office and Foodservice \n Coffee')
    // Order and Pick Up
    const pick_up = ref('Order and Pick Up')
    const order_app = ref('Order on the App')
    const order_web = ref('Order on the Web')
    const delivery = ref('Delivery')
    const order_options = ref('Order and Pick Up \n Options')
    const Explore = ref('Explore and Find Coffee \n for Home')
    // bottom menu
    const privacy = ref('Privacy Notice')
    const terms = ref('Terms of Use')
    const do_not = ref('Do Not Share My Personal Information')
    const ca_supply = ref('CA Supply Chain Act')
    const cookie = ref('Cookie Preferences')
</script>

<template>
    <div class="info">
    <!-- pc menu -->
    <div class="info_pc" width="100%">
    <!-- About Us pc menu -->
    <div class="info_about">
        <div class="info-title">{{ about_us }}</div>
        <a href="https://www.starbucks.com/about-us/">
        <div class="info-text">{{ our_company }}</div></a>
        <a href="https://www.starbucks.com/coffee/">
        <div class="info-text">{{ our_coffee }}</div></a>
        <a href="https://stories.starbucks.com/">
        <div class="info-text">{{ stories }}</div></a>
        <a href="https://archive.starbucks.com/">
        <div class="info-text">{{ starbucks_archive }}</div></a>
        <a href="https://investor.starbucks.com/ir-home/default.aspx">
        <div class="info-text">{{ investor_relations }}</div></a>
        <a href="https://customerservice.starbucks.com/sbux">
        <div class="info-text">{{ customer_service }}</div></a>
        <a href="https://www.starbucks.com/contact/">
        <div class="info-text">{{ contact_us }}</div></a>
    </div>
    <!-- Careers pc menu -->
    <div class="info_careers">
        <div class="info-title">{{ careers }}</div>
        <a href="https://www.starbucks.com/careers/working-at-starbucks/culture-and-values/">
        <div class="info-text">{{ culture }}</div></a>
        <a href="https://stories.starbucks.com/stories/inclusion-diversity/">
        <div class="info-text">{{ inclusion }}</div></a>
        <a href="https://www.starbucks.com/careers/working-at-starbucks/education/">
        <div class="info-text">{{ college }}</div></a>
        <a href="https://alumni.starbucks.com/login/">
        <div class="info-text">{{ alumni_community }}</div></a>
        <a href="https://www.starbucks.com/careers/">
        <div class="info-text">{{ us_careers }}</div></a>
        <a href="https://www.starbucks.com/careers/international-careers/">
        <div class="info-text">{{ international }}</div></a>
    </div>
    <!-- Social Impact pc menu -->
    <div class="info_social">
        <div class="info-title">{{ social_impact }}</div>
        <a href="https://www.starbucks.com/responsibility/people/">
        <div class="info-text">{{ people }}</div></a>
        <a href="https://www.starbucks.com/responsibility/planet/">
        <div class="info-text">{{ planet }}</div></a>
        <a href="https://www.starbucks.com/responsibility/reporting-hub/">
        <div class="info-text">{{ environmental }}</div></a>
    </div>
    <!-- For Business Partners pc menu -->
    <div class="info_partners">
        <div class="info-title">{{ business_partners }}</div>
        <a href="https://www.starbucks.com/business/landlord-faq/">
        <div class="info-text">{{ landlord }}</div></a>
        <a href="https://www.starbucks.com/business/suppliers/">
        <div class="info-text">{{ suppliers }}</div></a>
        <a href="https://www.starbuckscardb2b.com/s/">
        <div class="info-text">{{ corporate }}</div></a>
        <a href="https://www.nestlecoffeepartnerssl.com/our-brands/we-proudly-serve-starbucks-coffee-program">
        <div class="info-text">{{ office }}</div></a>
    </div>
    <!-- Order and Pick Up pc menu -->
    <div class="info_order">
        <div class="info-title">{{ pick_up }}</div>
        <a href="https://www.starbucks.com/rewards/mobile-apps/">
        <div class="info-text">{{ order_app }}</div></a>
        <a href="https://www.starbucks.com/menu">
        <div class="info-text">{{ order_web }}</div></a>
        <a href="https://www.starbucks.com/ways-to-order/delivery/">
        <div class="info-text">{{ delivery }}</div></a>
        <a href="https://www.starbucks.com/ways-to-order/">
        <div class="info-text">{{ order_options }}</div></a>
        <a href="https://athome.starbucks.com/?utm_source=starbucks.com&utm_medium=referral&utm_campaign=footer">
        <div class="info-text">{{ Explore }}</div></a>
    </div>
    </div>
    <!-- mobile menu -->
    <div class="mobilemenu_accordion">
    <!-- About Us mobile menu-->
    <details class="accordion_menu">
        <summary>About Us</summary>
        <p><a href="https://www.starbucks.com/about-us/">Our Company</a></p>
        <p><a href="https://www.starbucks.com/coffee/">Our Coffee</a></p>
        <p><a href="https://stories.starbucks.com/">Stories and News</a></p>
        <p><a href="https://archive.starbucks.com/">Starbucks Archive</a></p>
        <p><a href="https://investor.starbucks.com/ir-home/default.aspx">Investor Relations</a></p>
        <p><a href="https://customerservice.starbucks.com/sbux">Customer Service</a></p>
        <p><a href="https://www.starbucks.com/contact/">Contact Us</a></p>
    </details>
    <!-- Careers mobile menu -->
    <details class="accordion_menu">
        <summary>Careers</summary>
        <p><a href="https://www.starbucks.com/careers/working-at-starbucks/culture-and-values/">Culture and Values</a></p>
        <p><a href="https://stories.starbucks.com/stories/inclusion-diversity/">Inclusion, Diversity, and Equity</a></p>
        <p><a href="https://www.starbucks.com/careers/working-at-starbucks/education/">College Achievement Plan</a></p>
        <p><a href="https://alumni.starbucks.com/login/">Alumni Community</a></p>
        <p><a href="https://www.starbucks.com/careers/">U.S. Careers</a></p>
        <p><a href="https://www.starbucks.com/careers/international-careers/">International Careers</a></p>
    </details>
    <!-- Social Impact mobile menu -->
    <details class="accordion_menu">
        <summary>Social Impact</summary>
        <p><a href="https://www.starbucks.com/responsibility/people/">People</a></p>
        <p><a href="https://www.starbucks.com/responsibility/planet/">Planet</a></p>
        <p><a href="https://www.starbucks.com/responsibility/reporting-hub/">Environmental and Social Impact Reporting</a></p>
    </details>
    <!-- For Business Partners mobile menu -->
    <details class="accordion_menu">
        <summary>For Business Partners</summary>
        <p><a href="https://www.starbucks.com/business/landlord-faq/">Landlord Support Center</a></p>
        <p><a href="https://www.starbucks.com/business/suppliers/">Suppliers</a></p>
        <p><a href="https://www.starbuckscardb2b.com/s/">Corporate Gift Card Sales</a></p>
        <p><a href="https://www.nestlecoffeepartnerssl.com/our-brands/we-proudly-serve-starbucks-coffee-program">Office and Foodservice Coffee</a></p>
    </details>
    <!-- Order and Pick Up mobile menu -->
    <details class="accordion_menu">
        <summary>Order and Pick Up</summary>
        <p><a href="https://www.starbucks.com/rewards/mobile-apps/">Order on the App</a></p>
        <p><a href="https://www.starbucks.com/menu">Order on the Web</a></p>
        <p><a href="https://www.starbucks.com/ways-to-order/delivery/">Delivery</a></p>
        <p><a href="https://www.starbucks.com/ways-to-order/">Order and Pick Up Options</a></p>
        <p><a href="https://athome.starbucks.com/?utm_source=starbucks.com&utm_medium=referral&utm_campaign=footer">Explore and Find Coffee for Home</a></p>
    </details>
    </div>
    <!-- SNS icon -->
    <ul style="list-style: none;" class="sns_icon">
        <li><a href="https://open.spotify.com/user/starbucks"><img src="@/assets/spotify_icon.svg" alt="Spotify"></a></li>
        <li><a href="https://www.facebook.com/Starbucks/"><img src="@/assets/facebook_icon.svg" alt="Facebook"></a></li>
        <li><a href="https://www.pinterest.com/starbucks/"><img src="@/assets/pinterest_icon.svg" alt="Pinterest"></a></li>
        <li><a href="https://instagram.com/starbucks"><img src="@/assets/instagram_icon.svg" alt="Instagram"></a></li>
        <li><a href="https://www.youtube.com/starbucks"><img src="@/assets/youtube_icon.svg" alt="Youtube"></a></li>
        <li><a href="https://twitter.com/starbucks/"><img src="@/assets/twitter_icon.svg" alt="Twitter"></a></li>
    </ul>    
    <!-- bottom menu -->
    <div class="subinfo">
        <ul>
        <li class="subinfo-text"><a href="https://www.starbucks.com/terms/privacy-policy/">
        {{ privacy }}</a></li>
        <li class="subinfo-text"><a href="https://www.starbucks.com/terms/starbucks-terms-of-use/">
        {{ terms }}</a></li>
        <li class="subinfo-text"><a href="https://www.starbucks.com/personal-information">
        {{ do_not }}</a></li>
        <li class="subinfo-text"><a href="https://globalassets.starbucks.com/assets/A2A072E3411C4A6ABAEB8D6BCF286F43.pdf">
        {{ ca_supply }}</a></li>
        <li class="subinfo-text">{{ cookie }}</li>
        </ul>
    </div>
    </div>
</template>

<style scoped>
    *{
        font-family: SoDoSans;
    }
    .info{
        width: 100%;
        margin: 30px 0;
    }
    .info_pc{
        display: flex;
    }
    .info-title{
        width: 100%;
        margin-top: 20px;
        margin-right: 100px;
        font-size: 17px;
    }
   .info-text{
        width: 100%;
        margin-top: 20px;
        margin-right: 100px;
        color: rgb(118, 118, 118);
   }
   .info-text:hover{
        color: rgb(33, 33, 33);
   }
   /* SNS icon */
   .sns_icon{
        display: flex;
        margin: 30px 0;
   }
   .sns_icon img{
        width: 35px;
        height: 35px;
        margin-right: 15px;
   }
   /* bottom menu */
    .subinfo ul{
        padding-left: 0;
        list-style: none;
        display: inline-block;
    }
    .subinfo li{
        color: black;
        text-align: left;
        height: 30px;
        padding: 1.5em 2em;
    }
    li:hover{
        text-decoration: underline;
    }
    .subinfo a{
        color: black;
    }
    /* mobile */
    @media screen and (max-width:375px){
        .info_pc{
            display: none;
        }
        .accordion_menu{
            max-width: 100%;
            margin-bottom: 7px;            
        }
        /* title */
        .accordion_menu summary {
            display: flex;
            justify-content: space-between;
            align-items: center;
            position: relative;
            padding: 1.5em 2em;
            color: #333333;
            cursor: pointer;
        }
        .accordion_menu summary::-webkit-details-marker {
            display: none;
        }
        /* accordion menu open */
        .accordion_menu summary::after {
            transform: rotate(45deg);
            width: 10px;
            height: 10px;
            margin-left: 10px;
            border-bottom: 3px solid #333333b3;
            border-right: 3px solid #333333b3;
            content: '';
            transition: transform .3s;
        }
        /* accordion menu open mark */
        .accordion_menu[open] summary::after {
            transform: rotate(225deg);
        }
        .accordion_menu p {
            transform: translateY(-10px);
            opacity: 0;
            margin: 0;
            padding: 1em 2em 1.5em;
            transition: transform .5s, opacity .5s;
        }
        .accordion_menu[open] p {
            transform: translate;
            transition: transform .5s;
            opacity: 1;
        }
        .accordion_menu a{
            color: rgb(118, 118, 118);
        }
        .accordion_menu a:hover{
            color: black;
        }
    }
    /* pc */
    @media screen and (min-width:376px){
        .mobilemenu_accordion{
            display: none;
        }
        .info_pc{
            width: auto;
        }
        .subinfo ul{
            list-style-type: none;
            margin: 20px auto 0;
            text-align:center;
        }
        .subinfo li{
            float:left;
            padding: 0 10px 0 10px;}
        .subinfo li + li {
            border-left: 1px solid #333;
            padding: 0 10px 0 10px;
        }
    }
</style>