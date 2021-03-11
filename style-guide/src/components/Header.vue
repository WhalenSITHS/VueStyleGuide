<template>
  <h1><slot></slot></h1>
</template>

<script>
export default {
  name: "HeaderOne",
};
</script>

<style lang="scss">
h1 {
  color: var(--red);
  font-size: var(--h1);
}
</style>
<docs>
This is the header-one

## Examples
Sample

```jsx
<HeaderOne>Sample Text </HeaderOne>
```

</docs>
