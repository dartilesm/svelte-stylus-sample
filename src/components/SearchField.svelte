<script>
    import Icon from './Icon.svelte'
    export let placeholder
</script>

<div class="search">
    <input type="text" class="search__input" {placeholder} />
    <div class="search__button">
      <Icon data={{icon: 'assets/lupa.png'}} />
    </div>
</div>

<style lang="stylus">
.search
    width 100%
    height 45px
    background #fff
    box-shadow 0px 2px 4px rgba(140, 162, 174, 0.2)
    border-radius 12px
    display inline-flex
    .search__input
        width calc(100% - 45px)
        border none
        outline none
        height 100%
        border-radius 12px
        padding 12px 17px
        box-sizing border-box
    .search__button
        position relative
        display flex
        cursor pointer
        justify-content center
        align-items center
        height 100%
        width 45px
        background #FFC431
        border-radius 12px
</style>