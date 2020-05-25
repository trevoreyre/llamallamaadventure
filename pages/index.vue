<script>
import { Container, H2, P } from '@slate-ui/core'

export default {
  components: { Container, H2, P },
}
</script>
<template>
  <Container :class="$style.container">
    <H2 as="h1" mt="5xl" mb="lg">👋🏼 HELLO! WE’RE THE EYRES.</H2>
    <P>
      Trevor is a software engineer, and Lia is a stay at home mom to baby girl
      Lennon, and our two pups, Banana Pig and Mango Salsa. We moved into an RV
      in July, and come summer 2020 we’re hitting the road to travel full time.
      Stay tuned to follow along in our adventure!
    </P>
  </Container>
</template>

<style module>
.container {
  text-align: center;
  max-width: var(--breakpoint-sm);
}
</style>
