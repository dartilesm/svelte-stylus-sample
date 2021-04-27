<script>
    export let location
</script>

<section class="store-location store-location--margin-top-40">
    <h2 class="store-location__text">
      <b class="store-location__text-bold">Seleciona tu tienda</b>
    </h2>
    <a href="#" class="store-location__link">
      <img src="assets/location/ubicacion.png" alt="location icon" class="store-location__icon-location" />
      <span class="store-location__address">{location}</span>
    </a>
</section>

<style lang="stylus">
.store-location
    width 100%
    padding 0 20px
    box-sizing border-box
    color #44535B
    &.store-location--margin-top-40
        margin-top 40px
    .store-location__link
        color #00AF71!important
        text-decoration none
        font-size 1.2em
        display flex
        align-items center
        font-weight 500
    .store-location__address
        padding-left 5px
</style>