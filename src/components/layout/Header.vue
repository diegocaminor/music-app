<template lang="pug">
  section.hero.is-success
    .hero-head
      header.navbar
        .container
          .navbar-brand
            a.navbar-item
              strong 📻  Music App
            span.navbar-burger.burger(data-target='navbarMenuHeroA')
              span
              span
              span
          #navbarMenuHeroA.navbar-menu
            .navbar-end
              a.navbar-item(@click="selectLanguage('en')") 🇺🇸
              a.navbar-item(@click="selectLanguage('es')") 🇪🇸
              a.navbar-item.is-active
                router-link.nav-item(to="search") {{ $t('search') }}
              a.navbar-item
                router-link.nav-item(to="about") {{ $t('about') }}
    .hero-body
      .container.has-text-centered
        h1.title Music App
        h2.subtitle Canciones que estan Vue-nisimas!
        pm-player
</template>

<script>
import PmPlayer from "@/components/Player.vue";

export default {
  components: { PmPlayer },
  methods: {
    selectLanguage(lang) {
      this.$i18n.locale = lang;
    },
  },
};
</script>
