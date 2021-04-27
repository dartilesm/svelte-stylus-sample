<script>
	import Header from './components/Header.svelte'
	import StoreLocation from './components/StoreLocation.svelte'
	import CategoriesList from './components/CategoriesList.svelte'
	import StoreList from './components/StoreList.svelte'
	import Footer from './components/Footer.svelte'

const ICON_LIST = [
  {
    icon: 'assets/categories/super.png',
    text: 'Supermercado',
    selected: true,
    padding: true
  },
  {
    icon: 'assets/categories/carniceria.png',
    text: 'Carnicería',
    selected: false,
    padding: true
  },
  {
    icon: 'assets/categories/pharma.png',
    text: 'Farmacia',
    selected: false,
    padding: true
  }
]

const STORE_LIST = [
  {
    store: 'delicateck',
    discount: 20,
    title: 'Delicateck Caracas',
    category: 'Supermercado',
    stars: '4.5',
    deliveryTime: '3 días'
  },
  {
    store: 'lomas',
    discount: 20,
    title: 'Lomas Supermercado',
    category: 'Supermercado',
    stars: '4.5',
    deliveryTime: '3 días'
  }
]
</script>

<Header />
<StoreLocation location="Caracas, Ajuro"/>
<CategoriesList iconList={ICON_LIST} />
<StoreList stores={STORE_LIST} />
<Footer />