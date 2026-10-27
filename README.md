# Box Builder Lite

A step-by-step gift box builder for a Squarespace 7.1 product page. This repo only hosts the built script; the store's settings live in its Code Injection.

Settings → Developer Tools → Code Injection → Footer:

```html
<script>
window.BOX_CONFIG = {
  product: "/shop/p/gift-box",
  steps: [
    { title: "Hat or bow", heading: "Add a hat or bow", products: ["/shop/p/knot-hat", "/shop/p/bow-headband"] }
  ]
};
</script>
<script src="https://cdn.jsdelivr.net/gh/tools-hulo-dev/box-builder-lite@v1.3.1/box-builder.js" integrity="sha384-r32g7tmXocceAfqr0b05XjTP6/GMZtcp+ZlLb5ixc0RWfe6RRE0cnY9eZjl29qbH" crossorigin="anonymous"></script>
```

The box product needs a product form with a Text Area "Box contents" (and "Gift message").
