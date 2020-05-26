<script>
import { Container, H2, H3, P } from '@slate-ui/core'
import { Link, Logo, Map } from '~/components'

export default {
  components: { Container, H2, H3, P, Link, Logo, Map },
}
</script>
<template>
  <div>
    <Container :class="$style.tagLine" size="lg" mb="2xl">
      <Logo />
      <div>
        <H2 as="h1" mb="lg">👋🏼 Hello! We're the Eyres.</H2>
        <P>
          <Link href="https://trevoreyre.com">Trevor</Link> is a software
          engineer, and <Link href="https://liaeyre.com">Lia</Link> is a stay at
          home mom to baby girl Lennon, and our two pups, Banana Pig and Mango
          Salsa. We moved into an RV in July 2019, and started travelling full
          time in the summer of 2020.
        </P>
      </div>
    </Container>
    <Container size="sm" mb="2xl">
      <H3 mb="lg">🚌 Follow along</H3>
      <P>
        Follow our adventure on the map below. See where we've been and where
        we're headed next. If you happen to be in the area, hit us up. We'd love
        to meet and have a beer 🍺
      </P>
    </Container>
    <Container size="md">
      <Map />
    </Container>
  </div>
</template>

<style module>
.tag-line {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(320px, 1fr));
  gap: var(--spacing-lg);
  align-items: center;
}
</style>
