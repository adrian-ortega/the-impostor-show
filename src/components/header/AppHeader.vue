<template>
  <header class="main-header">
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

export default {
  name: 'AppHeader',
  components: {
    AppNavigation,
    AppLogo
  }
}
</script>
