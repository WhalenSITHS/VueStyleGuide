<template>
  <button :style="getColor">
    <!-- @slot Use this slot to place the button content -->
    <slot></slot>
  </button>
</template>

<script>
export default {
  props: {
    size: {
      type: String,
      default: "Medium",
    },
    /**
     * Sets the button background color
     


     * Accepts primary, secondary and accent as options
     

     
     * can be overridden with theme switcher in :root
     */
    color: {
      type: String,
      default: "primary",
    },
    validator: (color) => ["primary", "secondary"].includes(color),
  },
  computed: {
    getColor() {
      const createButtonTheme = ({ backgroundColor }) => ({
        "--button-background": backgroundColor,
      });

      const primary = createButtonTheme({
        backgroundColor: "var(--button-primary)",
      });

      const secondary = createButtonTheme({
        backgroundColor: "var(--button-secondary)",
      });

      const colors = {
        primary,
        secondary,
      };

      return colors[this.color];
    },
  },

  name: "default-button",
};
</script>

<style lang="scss">
button {
  font-size: var(--h5);
  height: 5rem;
  color: var(--text-primary);
  border: 1px solid #fff;
  padding: 0.5rem 2.4rem;
  text-decoration: none;
  transition: all 0.4s;
  background-color: var(--button-background);
  border-radius: 3rem;
  transition: all 0.3s;
}
button:hover {
  border: 1px solid clear;
  cursor: pointer;
  color: var(--text-primary);
}
</style>
<docs>
This is my test button
## Examples

Test Button

```jsx
<default-button color="secondary">Sample Secondary </default-button>
```

    
   
</docs>
