<script setup>
const posts = [
    {
        title: '5 motivos para ver JoJô',
        description: 'Novas notícias sobre o mangá mais esperado do ano'
    },

    {
        title: '5 motivos para amar JoJô',
        description: 'Novas notícias sobre o mangá mais esperado do ano'
    },

    {
        title: '5 motivos para idolatrar JoJô',
        description: 'Novas notícias sobre o mangá mais esperado do ano'
    }

];
</script>

<template>
  <main>
    <div class="post_container--primary">
        <h1>Últimas do blog</h1>
        <div class="post_container--card" v-for="post in posts">
            <div class="post_card--title">
                {{ post.title }}
            </div>
            <div class="post_card--description">
                {{ post.description }}
            </div>
        </div>
        <span class="btn btn--link">Ver tudo</span>
    </div>
  </main>
</template>

<style scoped>
.post_container--primary {
    justify-content: center;
    display: grid;
}

.post_container--card{
    width: 100%;
    padding: 10px 0;
    cursor: pointer;
   
}

.post_card--title{
    font-size: 1.5rem;
    font-weight: bold;
    color: #8f8f8f;
}

.post_card--description{
    font-size: 1rem;
    font-weight: 300;
    color: gray;
}
</style>
