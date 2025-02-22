<template>
    <section id="about">
        <theHeader />
        <h2>About</h2>
        <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Velit dolorum ipsam culpa sunt alias quaerat, 
            facilis nisi eligendi eius omnis!</p>
        <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Velit dolorum ipsam culpa sunt alias quaerat, 
            facilis nisi eligendi eius omnis!</p>
    </section>
</template>

<script setup>
import theHeader from '@/components/the header/the header.vue';
    definePageMeta({
        layout: 'about'
    })
</script>

<style scoped>
    h2{
        margin-bottom: 20px;
        font-size: 36px;
    }
    p{
        margin: 20px 0;
    }
</style>