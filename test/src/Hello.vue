<template>
  <h1>{{say}}
    <slot></slot>
  </h1>
</template>

<script>
  export default {
  props: {
    say: {
      type: String,
      default: 'Hello'
    }
  }
}
</script>