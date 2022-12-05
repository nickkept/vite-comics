<script>
import MyNav from "./components/MyNav.vue"
import Jumbotron from "./components/Jumbotron.vue"
import CardComponent from "./components/CardComponent.vue"
import BlueSection from "./components/BlueSection.vue"
import TheFooter from "./components/TheFooter.vue"
import FooterNav from "./components/FooterNav.vue"
export default {
  components: {MyNav,Jumbotron,CardComponent,BlueSection,TheFooter,FooterNav}
}
</script>

<template>
<MyNav></MyNav>
<Jumbotron></Jumbotron>
<CardComponent></CardComponent>
<BlueSection></BlueSection>
<TheFooter></TheFooter>
<FooterNav></FooterNav>

</template>

<style lang="scss">
	@use "./styles/general.scss";
  
  
</style>
