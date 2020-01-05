<template>
    <div>
        <h1>Things I like</h1>
        <p>These are some of the things that I am excited about.</p>
        <Card title="Guitars" description="After work, I often relax by playing some heavy guitar riffs." image="kitara"/>
        <Card title="Boardgames" description="Playing boardgames with friends and family is always a blast!" image="viticulture"/>
        <Card title="Computer games" description="I love strategy and roleplaying games. Check out Disco Elysium and Thea 2: The Shattering." image="disco-elysium"/>
    </div>
</template>

<style lang="scss" scoped>

</style>

<script>
import Card from '~/components/Card'
export default {
    layout: 'main',
    components: {
        Card
    }
}
</script>