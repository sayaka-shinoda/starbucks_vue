<script setup>
    import{ ref } from 'vue'
    const headermenuA = ref('MENU')
    const headermenuB = ref('REWARDS')
    const headermenuC = ref('GIFT CARDS')
    const headermenuD = ref('Find a store')
    const headermenuE = ref('Sign in')
    const headermenuF = ref('Join now')
</script>

<template>
    <div class="header">
    <div class="header-left">
        <img src="@/assets/logo.png" alt="Logo" class="header_logo">
        <div class="leftMenu">{{ headermenuA }}</div>
        <div class="leftMenu">{{ headermenuB }}</div>
        <div class="leftMenu">{{ headermenuC }}</div>
        </div>
    <div class="header-right">
        <div class="rightMenu">{{ headermenuD }}</div>
        <div class="rightMenu">{{ headermenuE }}</div>
        <div class="rightMenu">{{ headermenuF }}</div>
        </div>
    </div>

</template>

<style>
.header{
    width: 100%;
    margin: 50px 50px;
}
.header-left{
    display: flex;
}
.leftMenu,.rightMenu{
    margin: 10px 20px;
    font-family: SoDoSans;
    font-weight: bold;
}
.header-right{
    display: flex;
    float: right;
}
</style>