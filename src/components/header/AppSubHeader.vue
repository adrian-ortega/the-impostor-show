<template>
  <div class="main-header__sub">
    <div class="container">
      <div class="notification">
        <AppIconRecording/>
        <p>Live now! &mdash; Watch
          <a href="#">Jamie's Stream</a>
          AND
          <a href="#">AO's Stream</a>
        </p>
      </div>
    </div>
  </div>
</template>

<script>
import AppIconRecording from '@/components/icons/AppIconRecording'

export default {
  name: 'AppSubHeader',
  components: {
    AppIconRecording
  }
}
</script>
