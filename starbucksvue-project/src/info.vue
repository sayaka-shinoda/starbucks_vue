<script setup>
    import{ ref } from 'vue'
    const subinfoA = ref('Privacy Notice')
    const subinfoB = ref('Terms of Use')
    const subinfoC = ref('Do Not Share My Personal Information')
    const subinfoD = ref('CA Supply Chain Act')
    const subinfoE = ref('Cookie Preferences')
</script>

<template>
    <div class="Info" width="100%">
    <div class="infoA">
        <div class="info-title">About Us</div>
        <div class="info-text">Our Company</div>
        <div class="info-text">Our Coffee</div>
        <div class="info-text">Stories and News</div>
        <div class="info-text">Starbucks Archive</div>
        <div class="info-text">Investor Relations</div>
        <div class="info-text">Customer Service</div>
        <div class="info-text">Contact Us</div>
    </div>
<div class="infoB">
        <div class="info-title">Careers</div>
        <div class="info-text">Culture and Values</div>
        <div class="info-text">Inclusion, Diversity, and<br>Equity</div>
        <div class="info-text">College Achievement<br>Plan</div>
        <div class="info-text">U.S. Careers</div>
        <div class="info-text">International Careers</div>
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
    <div class="subInfo">
        <div class="subinfo-text">{{ subinfoA }}</div>
        <div class="subinfo-text">{{ subinfoB }}</div>
        <div class="subinfo-text">{{ subinfoC }}</div>
        <div class="subinfo-text">{{ subinfoD }}</div>
        <div class="subinfo-text">{{ subinfoE }}</div>
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