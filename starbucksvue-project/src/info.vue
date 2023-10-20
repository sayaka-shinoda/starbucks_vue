<script setup>
    import{ ref } from 'vue'
    // bottom menu
    const privacy = ref('Privacy Notice')
    const terms = ref('Terms of Use')
    const do_not = ref('Do Not Share My Personal Information')
    const ca_supply = ref('CA Supply Chain Act')
    const cookie = ref('Cookie Preferences') 
    // About Us
    const about_us = ref('About Us')^M
    const our_company = ref('Our Company')^M
    const our_coffee = ref('Our Coffee')^M
    const stories = ref('Stories and News')^M
    const starbucks_archive = ref('Starbucks Archive')^M
    const investor_relations = ref('Investor Relations')^M
    const customer_service = ref('Customer Service')^M
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
</script>

<template>
    <div class="Info" width="100%">
    <!-- About Us -->
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
    <!-- Careers -->
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
    <!-- Social Impact -->
    <div class="info_social">
        <div class="info-title">{{ social_impact }}</div>
        <a href="https://www.starbucks.com/responsibility/people/">
        <div class="info-text">{{ people }}</div></a>
        <a href="https://www.starbucks.com/responsibility/planet/">
        <div class="info-text">{{ planet }}</div></a>
        <a href="https://www.starbucks.com/responsibility/reporting-hub/">
        <div class="info-text">{{ environmental }}</div></a>
    </div>
    <!-- For Business Partners -->
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
    <!-- Order and Pick Up -->
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
    <!-- bottom menu -->
    <div class="subInfo">
        <a href="https://www.starbucks.com/terms/privacy-policy/">
        <div class="subinfo-text">{{ privacy }}</div></a>
        <a href="https://www.starbucks.com/terms/starbucks-terms-of-use/">
        <div class="subinfo-text">{{ terms }}</div></a>
        <a href="https://www.starbucks.com/personal-information">
        <div class="subinfo-text">{{ do_not }}</div></a>
        <a href="https://globalassets.starbucks.com/assets/A2A072E3411C4A6ABAEB8D6BCF286F43.pdf">
        <div class="subinfo-text">{{ ca_supply }}</div></a>
        <div class="subinfo-text">{{ cookie }}</div>
    </div>
</template>

<style>
    .Info{
        display: flex;
    }
    .info-title{
        margin: 20px 30px;
        font-size: 17px;
        font-family: SoDoSans;
    }
   .info-text{
        margin: 20px 30px;
        color: rgb(107 107 107);
   }
   .info-text:hover{
        color: rgb(33, 33, 33);
   }
    .subInfo{
        display: flex;
    }
    .subinfo-text{
        margin: 20px 30px;
        font-family: SoDoSans;
    }
</style>