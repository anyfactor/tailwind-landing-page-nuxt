<template>
<div>
    <!-- <hero /> -->
    <!-- <teasers />
    <features />
    <prices /> -->
    <experience 
    :title="automation.title"
    :items="automation.items"
    :technology="automation.technology"
    />
    <!-- <carousel /> -->
    <call-to-action />
</div>

</template>

<script>
// import Hero from '@/components/Hero'
import CallToAction from '@/components/CallToAction'
import Experience from '@/components/Experience'
// import Carousel from '@/components/Carousel'
import automation from '~/static/automation.json'

export default {
    components: {
    // hero: Hero,
    'call-to-action': CallToAction,
    experience: Experience,
    // carousel: Carousel
    },
    data: function() {
        return {
            automation: automation
        }
    }
}
</script>

<style>
</style>