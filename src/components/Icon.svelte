<script>
    export let data
</script>

<div class="icon">
    <img src={data.icon} alt="supermercado" class="icon__icon" />
    {#if data.text}
        <span class="icon__name" class:icon__name--selected={data.selected}>{data.text}</span>
    {/if}
</div>

<style lang="stylus">
.icon
    display flex
    cursor pointer
    flex-direction column
    justify-content center
    align-items center
    .icon__name
        white-space nowrap
        overflow hidden
        text-overflow ellipsis
    .icon__name--selected
        color #00AF71
</style>