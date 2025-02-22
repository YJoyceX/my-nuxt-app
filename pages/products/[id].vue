<template>
    <div>
        <p>Product details for {{ id }}</p>
        <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. 
            Similique magni doloremque libero distinctio quos neque ut alias molestias dolor temporibus.</p>
    </div>
</template>

<script setup>
    const {id} = useRoute().params

    definePageMeta({
        layout: 'products'
    })
</script>

<style scoped>

</style>