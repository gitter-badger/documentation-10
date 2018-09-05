# Structure of a Component

A Vue component is made up of 3 parts (and these can all be in the same file or split up)
A basic summary is below, but it is best explained [here](https://vuejs.org/v2/guide/components.html)

1. HTML
This is made up of a `template` tag and contains a single element (that could have other elements inside it)

```
<template>
    <div>
        <ul>
            <li v-on:click="doThing" class='class1'>Thing </li>
            <li>{{stuff}}</li>
        </ul>
    </div>
</template>
```

2. Javascript (or similar: Typescript etc)
The Javascript here looks like this:
```
data() {
    return {
        stuff: "stuff"
    }
},
methods: {
    doThing() {
        console.log('thing')
    }
}
```

More things can be added in here (check the documentation) to handle when the component is loaded, reloaded or destroyed, as well as dealing with properties passed to it

3. CSS (or similar: SCSS etc)
Different flavours of CSS are handled here (as long as your app config handles this) but the key things to note are:
1. `scoped` means that you can reuse classes (or selectors etc) but the styling is specific to this component
2. You can link to an external file with `src` to stop your file from getting cluttered. In this app, it is done like this to separate the styling from the logic

