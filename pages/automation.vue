<template>
<div>
    <!-- <hero /> -->
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
// import Hero from '@/components/Hero'
import CallToAction from '@/components/CallToAction'
import Experience from '@/components/Experience'
// import Carousel from '@/components/Carousel'

export default {
    components: {
    // hero: Hero,
    'call-to-action': CallToAction,
    experience: Experience,
    // carousel: Carousel
    },
    data: function() {
        return {
        title: "Automation & Bots",
        items: ['Deep and Routine Ecommerce Site Scrape with Information and Images for Dropshipping Services that interacts with modals and dialogue boxes', 'Another Deep and Routing Ecommerce Site Scrape with Information and Images scraped for Dropshipping Services scrapes thousands of images and provides detailed information in categories', "Checking the changes in inventory and prices of a competition's Ecommerce store", 'Creating a price tracking automation script of a competition', 'Tool to check inventory changes and price changes with weekly automated scraping', 'Parsing and Mining XML Data > Creating PDF for sharing and Printing & HTML for web hosting', 'Automated customized entering of Wordpress product information without bothering to buy wordpress plugin(s)', 'Twitter post maker with web interface that outputs shortened URLs and predetermined and relevant tags', 'Unfollowing everyone Instagram', '[Finance/ Trading] Finding Robintrack most popular stocks and then looking for sentiment and following of those stocks on stocktwits. And finding robintrack and stockwits data on ATH stocks', '[Finance/ Trading] Generating CSV full of data based of Ticker and Date from sourcing from YFinance or proprietary API'],
        technology: ["Web Interaction: Request-HTML, Selenium, Beatiful Soup 4 & URLlib",
                       "GUI Interaction: PyInput, PyperClip",
                       "API Creation: Firebase & RESTful Flask",
                       "Bots: Discord, Reddit, Twitter etc",
                       "Software Interaction: MS Office",
                       "Script Setup Options: PDF instructions, Video Tutorial, Video Chat & Remote Assistance",
                       "API: Google Envrionment, Google sheets, Reddit, Twitter & more or less anything"]
        }
    }
}
</script>

<style>
</style>