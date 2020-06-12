<template>
<div>
    <hero />
    <!-- <teasers />
    <features />
    <prices /> -->
    <experience 
    :title="title"
    :items="items"
    />
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

export default {
    components: {
    hero: Hero,
    features: Features,
    teasers: Teasers,
    prices: Prices,
    'call-to-action': CallToAction,
    experience: Experience
    },
    data: function() {
        return {
        title: "Web Scraping",
        items: ['Finding active GoodReads users and scraping various information from each of the users’ library', 'Scraping online directory for website, email, and contact information of Danish woodworking companies', 'Latitude and longitude scraped of 5000 institutes', 'Wikipedia sidebar information scraped of 200 educational institutes', 'Directory scrape specific lawsuit information scrape', 'Ecommerce site scrape: 2,500 popular search term generation and associated review and other information', 'Over 20,000 product URLs scraped from an eCommerce site and displayed and hidden information scraped from each listing', 'Scraping product information of a car company', '3,000+ rows of information scraped which were protected with limits and were hidden', '3,000+ rows of entries of a large scale directory with individual information structured in a tabular format', 'Directory of scrape commercial contractor for subcontracting', 'Subcontracting & competition assessment based on geo-location', '1,200 DnD information Scraped', 'Scraping the backup data and pictures from a way back machine', 'Scraping the full catalog of products of an e-commerce for market research', 'Emergency Medical Supply directory for a Trust Based operation']
        }
    }
}
</script>

<style>
</style>