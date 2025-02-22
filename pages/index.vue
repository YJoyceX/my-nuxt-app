<template>
    <section class="container">
        <theHeader />
        <postPreview 
        v-for="post in posts"
        :key="post.id"
        :title="post.title"
        :excerpt="post.previewText"
        :thumbnailImage="post.thumbnailUrl"
        :id="post.id" />
    </section>
</template>

<script>
import postPreview from '@/components/blog/postPreview.vue';
import theHeader from '@/components/the header/the header.vue';
    export default{
        components:{
            postPreview,
            theHeader
        },
        data(){
            return{
                posts: [
                {
                    title: 'Toner Pad',
                    previewText: 'THEFACESHOP focuses on using natural ingredients from all over the world to nourish and revitalize your skin.',
                    thumbnailUrl: '/images/tonerPad.png',
                    id:"toner-pad"
                },
                {
                    title: 'The Therapy',
                    previewText: 'THEFACESHOP focuses on using natural ingredients from all over the world to nourish and revitalize your skin.',
                    thumbnailUrl: '/images/theTherapy.png',
                    id:"the-therapy"
                },
            ]
            };
        }
    };

    definePageMeta({
        layout: 'home'
    })
</script>

<style scoped>
.container {
  display: flex;
  flex-direction: column;
}
</style>