# vuejs-tipsy-example

Bootstrapped with webpack-simple, a project template for vue-cli: https://github.com/vuejs-templates/webpack-simple

## Usage

``` bash
$ npm install
$ npm run dev
```

## Key parts

Import libraries inside the vue component:

``` javascript
import $ from 'jquery'
import tipsy from 'jtipsy'
```

Add jQuery as a plugin for Webpack:

```javascript
plugins: [
  new webpack.ProvidePlugin({
    $: 'jquery',
    jQuery: 'jquery',
    'window.jQuery': 'jquery'
  })
]
```

Import tipsy styles from your component:
 
```less
<style lang="less">
  @import "../node_modules/jtipsy/src/jquery.tipsy.css";
</style>
```

Enjoy ;)
