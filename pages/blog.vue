<template>
  <div>
    <h1>Blog</h1>
    <div>
        <BlogPost v-for="post in reversedPosts" :key=post.index :post=post />
    </div>
  </div>
</template>

<script>
import BlogPost from "~/components/BlogPost"
export default {
  layout: 'main',
  components: {
      BlogPost
  },
  data () {
      return {
          blog: {
            posts: [
                {
                    index: 1,
                    title: "Hello World",
                    content: "Hello everyone, this is my first ever blogpost.",
                    date: "5.1.2020"
                },
                {
                    index: 2,
                    title: "Website under construction",
                    content: "The work on the website is going well, hopefully I will able to add to on a consistent basis.",
                    date: "5.1.2020"
                }
            ]
        }
      }
  },
  computed: {
      reversedPosts: function() {
          return this.blog.posts.reverse();
      }
  }
}
</script>