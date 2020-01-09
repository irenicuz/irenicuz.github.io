<template>
    <div class="card">
        <img :src="cardImage">
        <div class="contents">
            <h2>{{ title }}</h2>
            <p>{{ description }}</p>
        </div>
    </div>
</template>

<style lang="scss" scoped>
    .card {
        //max-width: 500px;
        display: flex;

        margin-bottom: 20px;
        .contents {
            padding: 20px;

            h2 {
                margin-bottom: 10px;
            }
        }

        img {
            //max-width: 300px;
            //max-height: 150px;
            width: 160px;
        }
    }
</style>

<script>
export default {
    props: [ "title", "description", "image" ],
    computed: {
        cardImage () {
            if(this.image){
                return require(`~/assets/img/${this.image}.svg`)
            }
        }
    }
}
</script>