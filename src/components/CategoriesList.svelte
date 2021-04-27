<script>
    import Icon from './Icon.svelte'

    export let iconList
</script>

<section class="categories-list">
    {#each iconList as icon}
        <div class="categories-list__item">
            <Icon data={icon} />
        </div>
    {/each}
</section>

<style lang="stylus">
.categories-list
    padding 0 20px
    width 100%
    box-sizing border-box
    display flex
    justify-content center
    overflow auto
    color #44535B
    .categories-list__item 
        padding 0 20px

</style>