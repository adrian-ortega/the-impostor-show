<template>
  <div class="hero-starry-night" ref="container">
    <span
      v-for="i in max"
      :key="i"
      :class="getStarClasses()"
      :style="getStarPosition()"
    ></span>
  </div>
</template>

<script>
export default {
  name: 'HeroStarryNight',
  data () {
    return {
      max: 269,
      width: 0,
      height: 0,
      style: {},
      types: [
        'star--a',
        'star--b',
        'star--c',
        'star--d'
      ]
    }
  },
  methods: {
    getStarClasses () {
      return ['star'].concat(this.types[Math.floor(Math.random() * this.types.length)])
    },

    getStarPosition () {
      const animationDelay = `${Math.round(Math.random() * 2000)}ms`
      const animationDuration = `${(Math.round(Math.random() * 2000) + 500)}ms`

      return {
        top: `${Math.round(Math.random() * this.style.height)}px`,
        left: `${Math.round(Math.random() * this.style.width)}px`,
        animationDelay,
        animationDuration
      }
    },

    watchContainerChanges () {
      window.addEventListener('resize', () => this.setContainerDimensions())
    },

    setContainerDimensions () {
      this.style = {
        width: this.$el.offsetWidth,
        height: this.$el.offsetHeight
      }
    }
  },
  mounted () {
    this.setContainerDimensions()
    this.watchContainerChanges()
  }
}
</script>
