<script>
    import Icon from './Icon.svelte'

    const LEFT_ICON_LIST = [
    {
        icon: 'assets/footer/store.png',
        padding: true,
        text: 'Tiendas',
        selected: true
    },
    {
        icon: 'assets/footer/location.svg',
        padding: true,
        text: 'Caracas'
    }
]

const CENTERED_ICON = {
    icon: 'assets/footer/cart.svg',
    roundedShadow: true
}

const RIGHT_ICON_LIST = [
    {
        icon: 'assets/footer/money.svg',
        padding: true,
        text: 'Gana $5.00'
    },
    {
        icon: 'assets/footer/user.svg',
        padding: true,
        text: 'Iniciar Sesión'
    }
]
</script>

<footer class="footer">
    <div class="footer__icon-center">
        <div class="footer__icon-center-container">
            <Icon data={CENTERED_ICON} />
        </div>
    </div>
    <div class="footer__container">
      <div class="footer__icon-left">
          {#each LEFT_ICON_LIST as data}
            <Icon {data} />
          {/each}        
      </div>
      <div class="footer__icon-right">
        {#each RIGHT_ICON_LIST as data}
            <Icon {data} />
        {/each}        
      </div>
    </div>
</footer>

<style lang="stylus">
.footer
    position relative
    height 86px
    width 100%
    color #44535B
    .footer__container
        position absolute
        bottom 0
        height calc(100% - 10px)
        width 100%
        display flex
        justify-content space-between
        overflow hidden
        background #FFFFFF
        border-radius 20px 20px 0 0
        box-shadow 0px -2px 4px rgba(140, 162, 174, 0.2)
        .footer__icon-left, .footer__icon-right
            display inline-flex
            width 40%
            justify-content space-around
    .footer__icon-center
        top -5px
        width 20%
        position absolute
        left 50%
        transform translateX(-50%)
        display flex
        justify-content center
        z-index 1
        .footer__icon-center-container 
            padding 20px
            border-radius 20px
            background-color white
            box-shadow 2px 2px 10px rgba(140, 162, 174, 0.2)
</style>