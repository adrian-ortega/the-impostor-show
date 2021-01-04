<template>
  <div class="view view--home">
    <AppHeader/>
    <AppFooter/>
  </div>
</template>

<script>
import AppHeader from '@/components/header/AppHeader'
import AppFooter from '@/components/footer/AppFooter'

export default {
  name: 'Home',
  components: {
    AppHeader,
    AppFooter
  }
}
</script>
