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
        <div class="info-text">{{ our_company }}</div>
        <div class="info-text">{{ our_coffee }}</div>
        <div class="info-text">{{ stories }}</div>
        <div class="info-text">{{ starbucks_archive }}</div>
        <div class="info-text">{{ investor_relations }}</div>
        <div class="info-text">{{ customer_service }}</div>
        <div class="info-text">{{ contact_us }}</div>
    </div>
    <!-- Careers -->
    <div class="info_careers">
        <div class="info-title">{{ careers }}</div>
        <div class="info-text">{{ culture }}</div>
        <div class="info-text">{{ inclusion }}</div>
        <div class="info-text">{{ college }}</div>
        <div class="info-text">{{ alumni_community }}</div>
        <div class="info-text">{{ us_careers }}</div>
        <div class="info-text">{{ international }}</div>
    </div>
    <!-- Social Impact -->
    <div class="info_social">
        <div class="info-title">{{ social_impact }}</div>
        <div class="info-text">{{ people }}</div>
        <div class="info-text">{{ planet }}</div>
        <div class="info-text">{{ environmental }}</div>
    </div>
    <!-- For Business Partners -->
    <div class="info_partners">
        <div class="info-title">{{ business_partners }}</div>
        <div class="info-text">{{ landlord }}</div>
        <div class="info-text">{{ suppliers }}</div>
        <div class="info-text">{{ corporate }}</div>
        <div class="info-text">{{ office }}</div>
    </div>
    <!-- Order and Pick Up -->
    <div class="info_order">
        <div class="info-title">{{ pick_up }}</div>
        <div class="info-text">{{ order_app }}</div>
        <div class="info-text">{{ order_web }}</div>
        <div class="info-text">{{ delivery }}</div>
        <div class="info-text">{{ order_options }}</div>
        <div class="info-text">{{ Explore }}</div>
    </div>
    </div>
    <!-- bottom menu -->
    <div class="subInfo">
        <div class="subinfo-text">{{ privacy }}</div>
        <div class="subinfo-text">{{ terms }}</div>
        <div class="subinfo-text">{{ do_not }}</div>
        <div class="subinfo-text">{{ ca_supply }}</div>
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
   }
    .subInfo{
        display: flex;
    }
    .subinfo-text{
        margin: 20px 30px;
        font-family: SoDoSans;
    }
</style>