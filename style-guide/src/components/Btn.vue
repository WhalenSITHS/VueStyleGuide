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
  height: 50px;
  width: 500px;
  border-radius: 10px;
  font-size: 50px;
  background-color: blue;
  transition: all 0.3s;
}
button:hover {
  background-color: red;
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