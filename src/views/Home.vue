<template>
  <div class="view view--home">
    <AppHeader/>
    <AppHomeHero/>
    <AppFooter/>
  </div>
</template>

<script>
import AppHeader from '@/components/header/AppHeader'
import AppFooter from '@/components/footer/AppFooter'
import AppHomeHero from '@/components/hero/AppHomeHero'

export default {
  name: 'Home',
  components: {
    AppHomeHero,
    AppHeader,
    AppFooter
  }
}
</script>
