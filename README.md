# \<coindesk-component\>

Provides a simple Webcomponent to make its Bitcoin Price Index (BPI) available to others


Example:
<!---
```
<custom-element-demo>
  <template>
    <script src="../webcomponentsjs/webcomponents-lite.js"></script>    
    <link rel="import" href="bitcoin-price.html">
    <next-code-block></next-code-block>
  </template>
</custom-element-demo>
```
-->
```html
<template is="dom-bind">
<bitcoin-price currency="BRL" updated="{{updated}}" updatediso="{{updatediso}}" updateduk="{{updateduk}}" disclaimer="{{disclaimer}}"
    code="{{code}}" rate="{{rate}}" description="{{description}}" rate_float="{{rate_float}}"></bitcoin-price>

<br/> Code:{{code}}
<br/> Description:{{description}}
<br/> Rate:{{rate}}
<br/>Updated:{{updated}}
<br/> Disclaimer:{{disclaimer}}
</template>
```

## Install the Polymer-CLI

First, make sure you have the [Polymer CLI](https://www.npmjs.com/package/polymer-cli) installed. Then run `polymer serve` to serve your application locally.

## Viewing Your Application

```
$ polymer serve
```

## Building Your Application

```
$ polymer build
```

This will create a `build/` folder with `bundled/` and `unbundled/` sub-folders
containing a bundled (Vulcanized) and unbundled builds, both run through HTML,
CSS, and JS optimizers.

You can serve the built versions by giving `polymer serve` a folder to serve
from:

```
$ polymer serve build/bundled
```

## Running Tests

```
$ polymer test
```

Your application is already set up to be tested via [web-component-tester](https://github.com/Polymer/web-component-tester). Run `polymer test` to run your application's test suite locally.
