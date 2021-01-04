<template>
  <div class="navigation-menu">
    <div class="navigation-end">
    <template v-for="(item, i) in items">
      <div class="navigation-item" :key="i">
        <router-link
          class="navigation-link"
          :to="item.to"
          :title="item.title"
          exact-active-class="is-active"
        >
          <span class="navigation-link__text">
            {{item.text}}
          </span>
        </router-link>
      </div>
    </template>
    </div>
  </div>
</template>

<script>
export default {
  name: 'AppNavigation',
  data () {
    return {
      items: [
        {
          text: 'Episodes',
          title: 'Episodes List',
          to: {
            name: 'home'
          }
        },
        {
          text: 'About',
          title: 'About The Impostor Show',
          to: {
            name: 'home'
          }
        },
        {
          text: 'Contact',
          title: 'Contact The Impostor Show',
          to: {
            name: 'home'
          }
        }
      ]
    }
  }
}
</script>
