<template>
  <div style="border:1px solid red;width:400px">
    <MDXProvider :mdxComponents="mdxComponents">
      <slot></slot>
    </MDXProvider>
  </div>
</template>

<script>
  import MDXProvider from './MDXProvider.vue';
  import H1 from './H1.vue';
  import Hello from './Hello.vue'
  import Counter from './Counter.vue';
  const mdxComponents = {
  h1: H1,
  "my-counter" : Counter,
  Counter : Counter,
  Hello
};
  export default {
  components: {MDXProvider},
  setup(){
    return { mdxComponents }
  }
}
</script>