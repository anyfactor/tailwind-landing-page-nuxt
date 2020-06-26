<template>
<div>
    <hero />
    <!-- <teasers />
    <features />
    <prices /> -->
    <experience 
    :title="title"
    :items="items"
    :technology="technology"
    />
    <!-- <carousel /> -->
    <call-to-action />
</div>

</template>

<script>
import Hero from '@/components/Hero'
import Features from '@/components/Features'
import Teasers from '@/components/Teasers'
import Prices from '@/components/Prices'
import CallToAction from '@/components/CallToAction'
import Experience from '@/components/Experience'
// import Carousel from '@/components/Carousel'

export default {
    components: {
    hero: Hero,
    features: Features,
    teasers: Teasers,
    prices: Prices,
    'call-to-action': CallToAction,
    experience: Experience,
    // carousel: Carousel
    },
    data: function() {
        return {
        title: "Automation",
        items: ['Deep and Routine Ecommerce Site Scrape with Information and Images for Dropshipping Services that interacts with modals and dialogue boxes', 'Another Deep and Routing Ecommerce Site Scrape with Information and Images scraped for Dropshipping Services scrapes thousands of images and provides detailed information in categories', "Checking the changes in inventory and prices of a competition's Ecommerce store", 'Creating a price tracking automation script of a competition', 'Tool to check inventory changes and price changes with weekly automated scraping', 'Parsing and Mining XML Data > Creating PDF for sharing and Printing & HTML for web hosting', 'Automated customized entering of Wordpress product information without bothering to buy wordpress plugin(s)', 'Twitter post maker with web interface that outputs shortened URLs and predetermined and relevant tags', 'Unfollowing everyone Instagram'],
        technology: ["Web Interaction: Request-HTML, Selenium, Beatiful Soup 4 & URLlib",
                       "GUI Interaction: PyInput, PyperClip",
                       "API Creation: FastAPI, Flask & Firebase",
                       "Software Interaction: MS Office",
                       "Script Setup Options: PDF instructions, Video Tutorial, Video Chat & Remote Assistance",
                       "API: Google Envrionment, Google sheets, Reddit, Twitter & more or less anything"]
        }
    }
}
</script>

<style>
</style>