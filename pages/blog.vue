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
                    content: "Hello everyone, this is my first ever blogpost."
                },
                {
                    index: 2,
                    title: "Website under construction",
                    content: "The work on the website is going well, hopefully it will go live in a few weeks' time."
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