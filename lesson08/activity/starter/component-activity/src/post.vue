<template>
    <div id="app">
    <article class="post">
        <h3 class="post_title">{{ post.title }}</h3>
        <h6 class="post_author">{{ post.author }}</h6>
        <p class="post_excerpt">{{ post.excerpt }}</p>
        <button @click="post.likes++" class="post_likes">+1 | {{ post.likes }}</button>
    </article>
    </div>
</template>
  
<script>
    export default {
        name: 'postArray',
        props: ['posts'],
    }
</script>