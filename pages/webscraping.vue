<template>
<div>
    <!-- <hero /> -->
    <experience 
    :title="webscraping['title']"
    :items="webscraping['items']"
    :technology="webscraping['technology']"
    />
    <call-to-action />
</div>

</template>

<script>
// import Hero from '@/components/Hero'
import CallToAction from '@/components/CallToAction'
import Experience from '@/components/Experience'
import webscraping from '~/static/webscraping.json'

export default {
    components: {
    // hero: Hero,
    'call-to-action': CallToAction,
    experience: Experience
    },
    data: function() {
        return {
            webscraping: webscraping
        }
    }
}
</script>

<style>
</style>