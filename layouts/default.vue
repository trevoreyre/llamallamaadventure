<script>
import { Css } from '@slate-ui/core'

export default {
  components: { Css },
}
</script>

<template>
  <Css>
    <main :class="$style.main">
      <nuxt />
    </main>
  </Css>
</template>

<style module>
.main {
  display: block;
  padding: var(--spacing-2xl) var(--spacing-sm);
}
</style>

<style>
:root {
  --color-brand-500: #9fee80;
  --color-brand-700: #58c42e;
  --color-text-primary: #4e616c;
}

body {
  background: var(--color-background-light);
}

iframe {
  border: none;
  display: block;
  width: 100%;
}

p,
a {
  font-size: 1.25rem;
  line-height: 1.6;
}
</style>
