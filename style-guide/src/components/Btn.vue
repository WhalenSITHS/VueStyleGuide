<template>
  <button><slot></slot></button>
</template>

<script>
export default {
  name: "default-button",
};
</script>

<style lang="scss">
button {
  font-size: var(--h4);
  height: 5rem;
  color: var(--background-primary);
  border: 1px solid #fff;
  padding: 0.5rem 2.4rem;
  text-decoration: none;
  transition: all 0.4s;
  background-color: var(--text-primary);
  border-radius: 3rem;
  transition: all 0.3s;
}
button:hover {
  border: 1px solid clear;
  background-color: var(--background-primary);
  cursor: pointer;
  color: var(--text-primary);
}
</style>
<docs>
This is my test button
## Examples

Test Button

```jsx
<default-button>
  Sample Text
</default-button>
```

    
   
</docs>
