<template>
  <h1 style="background: teal;color:white">
    <slot></slot>
  </h1>
  <details v-if="$attrs.showComponents">
    <summary>mdxComponents</summary>
    <pre>{{ $mdxComponents }}</pre>
  </details>
</template>

<script>
  export default {
  inject: ['$mdxComponents'],
}
</script>