<script setup>
  const {data:blogPostList} = useAsyncData('blogPostList', ()=>{
    return queryContent('/blog').find()
  })
  console.log(blogPostList)
</script>

<template>
  <div class="container">
    <section class="articles">
      <div class="column is-8 is-offset-2">
        <div class="card article" v-for="post in blogPostList" :key="post.title"> 
          <NuxtLink :to="post._path">
            <section class="blog-post-card card article">
              <div class="media">
                <div class="media-content has-text-centered">
                
                  <h3 class="title article-title has-text-weight-bold">
                    {{ post.title }}
                  </h3>
                  <BlogPostMeta :author="post.author" />
                </div>
              </div>
              <div class="card-content">
                <div class="content article-body is-size-5">
                  {{  post.description }}
                </div>
              </div>
            </section>
          </NuxtLink>
        </div>
      </div>
    </section>
  </div>
</template>

<style>
.blog-post-card {
  padding-top: 2.5rem;
  padding-bottom: 3rem;
}

.blog-post-card .card-content {
  padding: 1rem;
}

.blog-post-card .title {
  margin-bottom: 1rem;
}
</style>
