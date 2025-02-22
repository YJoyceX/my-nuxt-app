<template>
    <section class="container">
        <theHeader />
    </section>
</template>

<script setup>
import theHeader from '@/components/the header/the header.vue';
    definePageMeta({
        layout: 'products'
    })
</script>

<style scoped>
.container {
  display: flex;
  flex-direction: column;
}
</style>