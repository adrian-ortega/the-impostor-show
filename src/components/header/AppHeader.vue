<template>
  <header class="main-header">
    <AppSubHeader/>
    <nav class="navigation">
      <div class="container">
        <div class="navigation-brand">
          <div class="navigation-item">
            <router-link :to="{ name: 'home' }">
              <AppLogo/>
            </router-link>
          </div>
        </div>
        <AppNavigation/>
      </div>
    </nav>
  </header>
</template>

<script>
import AppLogo from '@/components/logo/AppLogo'
import AppNavigation from '@/components/header/AppNavigation'
import AppSubHeader from '@/components/header/AppSubHeader'

export default {
  name: 'AppHeader',
  components: {
    AppSubHeader,
    AppNavigation,
    AppLogo
  }
}
</script>
