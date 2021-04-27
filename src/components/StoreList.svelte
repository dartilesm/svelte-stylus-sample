<script>
    import StoreCard from './StoreCard.svelte'

    export let stores
</script>

<section class="stores-list">
    {#each stores as data}
        <StoreCard {data} />
    {/each}
</section>

<style lang="stylus">
.stores-list
    display flex
    padding 30px 20px
    box-sizing border-box
    flex-wrap wrap
    justify-content center
</style>