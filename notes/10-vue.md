# Vue


Reactive is for objects only
Ref Is for primitive data types only

Computed watches the AppState for changes
ex.

```js
values: computed(() => AppState.values)
```

```html
<div class="col-3" v-for"v in values" :key="v.id">
 <Value :value="v">
</div>
```

<br>

## Props are like parameters to a function

### ex

```js
props: {
  value: {
    type: Value,
    required, true
  }
}
```

## MODALS

- Copy & Paste modal from bootstrap

- Change the modal header and modal body to have slots inside of them


2 APIs -- options and composition