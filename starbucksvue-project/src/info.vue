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
    <div class="infoC">
        <div class="info-title">Social Impact</div>
        <div class="info-text">People</div>
        <div class="info-text">Planet</div>
        <div class="info-text">Environmental and Social<br>Impact Reporting</div>
    </div>
    <div class="infoD">
        <div class="info-title">For Business Partners</div>       
        <div class="info-text">Landlord Support Center</div>
        <div class="info-text">Suppliers</div>
        <div class="info-text">Corporate Gift Card Sales</div>
        <div class="info-text">Office and Foodservice<br>Coffee</div>
    </div>
    <div class="infoE">
        <div class="info-title">Order and Pick Up</div>
        <div class="info-text">Order on the App</div>
        <div class="info-text">Order on the Web</div>
        <div class="info-text">Delivery</div>
        <div class="info-text">Order and Pick Up<br>Options</div>
        <div class="info-text">Explore and Find Coffee<br>for Home</div>
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