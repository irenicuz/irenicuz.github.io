<template>
    <div>
        <h1>Song of the moment</h1>
        <p>This might be my favorite song at the moment. Give it a listen!</p>
        <iframe width="560" height="315" src="https://www.youtube.com/embed/ARI0XyTiips" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
    </div>
</template>

<style lang="scss" scoped>

    iframe {
        margin: 30px 0;
    }

</style>

<script>
export default {
  layout: 'main',
}
</script>