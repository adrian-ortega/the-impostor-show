<template>
  <div class="main-hero main-hero--home">
    <div class="main-hero__content">
      <div class="container">
        <h1>
          <strong>A podcast about</strong>
          <span>whatever the f*ck we want</span>
        </h1>
      </div>
    </div>
    <div class="main-hero__background">
      <HeroStarryNight/>
    </div>
  </div>
</template>

<script>
import HeroStarryNight from '@/components/hero/HeroStarryNight'
export default {
  name: 'AppHomeHero',
  components: { HeroStarryNight }
}
</script>
