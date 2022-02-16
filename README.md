# Class (same) not generated during class binding for v-for/ngFor

For the following code the bg class will not be generated for the first 'div' element, [screenshot](./src/assets//class_binding_issue.png)

```js
const switches = [{
  on: true,
}, {
  on: false,
}]

```

```html
<div
    v-for="s of switches"
    class="w-32 h-32 border-2 border-dashed"
    :class="{ 'bg-pink-300': s.on, 'bg-pink-300': !s.on }"
></div>
```