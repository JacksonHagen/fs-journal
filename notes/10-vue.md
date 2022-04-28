<h1 style="color: aquamarine"><b>Vue</b></h1>

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

#### ex

```js
props: {
  value: {
    type: Value,
    required, true
  }
}
```
<hr>

## MODALS

- Copy & Paste modal from bootstrap

- Change the modal header and modal body to have slots inside of them

<hr>

2 APIs -- options and composition

<hr>
<hr>

<h2 style="color: aquamarine;"><b>REVIEW</b></h3>


- If it is used in the template, it needs to be in the setup's return

- Pages' only parent is the router

- watchEffect manipulates other values - "when this value changes, set this other value"

- computed returns a value - "only get me the results for this"

<h2 style="color: aquamarine;"><b>PROPS REVIEW</b></h3>

- <b>PAGES DON'T GET PROPS</b>

- Props are either required <b style="color: salmon">OR</b> default

- Props are only needed when theres more than one piece of data 

<hr>

## Setup example
```js
setup() {
  //variables that are needed but not in the template
  //NOTE PRIVATE VARIABLES
  const route = useRoute()
  return {
    //All Variables in the template MUST be in the return
    //local variables
    //computed values
    //methods
    createProject() {
      //methods can be defined inside or outside of the return object. 
      //If it is defined outside, it must be returned to be used in the template
    }
  }
}
```

- Account is always me - the person who is actively logged in. Private info

- Profile is anyone. Public info
