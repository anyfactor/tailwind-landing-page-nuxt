<template>
<div>
    <hero />
    <experience 
    :title="title"
    :items="items"
    :technology="technology"
    links
    />
    <call-to-action />
</div>

</template>

<script>
import Hero from '@/components/Hero'
import CallToAction from '@/components/CallToAction'
import Experience from '@/components/Experience'

export default {
    components: {
    hero: Hero,
    'call-to-action': CallToAction,
    experience: Experience
    },
    data: function() {
        return {
        title: "Data Analytics & Visualization",
        items: [{'name': 'Hour and Month submission statistics of top 995 posts of r/accounting', 'link': 'https://old.reddit.com/r/Accounting/comments/9cjy9s/hour_and_month_submission_statistics_of_top_995/'}, {'name': 'Percentage of submission month of top 995 all-time posts of r/accounting', 'link': 'https://old.reddit.com/r/Accounting/comments/9cj5bs/percentage_of_submission_month_of_top_995_all/'}, {'name': 'Days of the week of submission of top 500 posts of last year', 'link': 'https://old.reddit.com/r/dataisbeautiful/comments/9ce6y0/days_of_the_week_of_submission_of_top_500_posts/'}, {'name': 'Top 15 most commonly misspelt words on Reddit according to u/CommonMisspellingBot', 'link': 'https://old.reddit.com/r/dataisbeautiful/comments/9bk3h8/top_15_most_commonly_misspelled_words_on_reddit/'}, {'name': 'IMDB Top 250 Bollywood movies analysis; the number of movies per decade and average ratings', 'link': 'https://reddit.com/r/dataisbeautiful/comments/9jnq7n/imdb_top_250_bollywood_movies_number_of_movies/'}, {'name': 'Fortune 500 Headquarters web interactive data visualization through SVG (Web Interactive)', 'link': 'https://www.reddit.com/r/dataisbeautiful/comments/bvo6u1/distribution_of_fortune_500_headquarters_oc/'}, {'name': 'Frequency of the word "Trump: in 1000 titles in political and news subreddits', 'link': 'https://old.reddit.com/r/dataisbeautiful/comments/b0ltx0/mention_of_the_word_trump_in_in_the_top_1000_post/'}],
        technology: ['Python', 'Selenium, Requests-HTML', 'Requests, URLLib, Beautiful Soup 4', 'Regex', 'Pandas, Numpy', 'Microsoft Excel, Google Sheets', 'SQL']
        }
    }
}
</script>

<style>
</style>