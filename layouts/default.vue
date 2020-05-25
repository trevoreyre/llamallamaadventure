<script>
import { AppBar, Css } from '@slate-ui/core'
import Logo from '~/components/Logo.vue'

export default {
  components: { AppBar, Css, Logo },
}
</script>

<template>
  <Css>
    <AppBar :class="$style.appBar" theme="light">
      <NuxtLink to="/" :class="$style.logo">
        <Logo />
      </NuxtLink>
      <div>
        <NuxtLink to="/">
          Home
        </NuxtLink>
        <NuxtLink to="/">
          Contact
        </NuxtLink>
      </div>
    </AppBar>
    <nuxt />
  </Css>
</template>

<style module>
.app-bar.app-bar {
  --border: var(--border-none);
}

.logo {
  height: var(--spacing-7xl);
}
</style>

<style>
body {
  background: var(--color-background-light);
}
</style>
