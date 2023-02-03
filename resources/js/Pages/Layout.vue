
<script>
import { Link } from '@inertiajs/vue3'

export default {
    name:'Layout',
    components: {
        Link
    }
}
</script>

<template>
  <main>
    <header>
      <Link href="/">Home</Link>
      <Link href="/about">About</Link>
      <Link href="/contact">Contact</Link>
    </header>
    <article>
      <slot></slot>
    </article>
  </main>
</template>