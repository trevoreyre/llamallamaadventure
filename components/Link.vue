<script>
export default {
  props: {
    href: {
      type: String,
      required: true,
    },
  },
}
</script>

<template>
  <a :class="$style.link" :href="href" target="_blank" rel="noreferrer">
    <slot></slot>
  </a>
</template>

<style module>
.link {
  color: var(--color-brand-700);
  font-weight: var(--font-weight-bold);
}
</style>
