# webpack-rxjs-externals

Utility to generate all the ["externals"](https://webpack.github.io/docs/library-and-externals.html) for your webpack config.

Since RxJS is ever-changing, this removes the need to maintain a list, instead generating it on the fly.

#### webpack.config.js

```js
import createRxJSExternals from 'webpack-rxjs-externals';

export default {
  externals: {
    ...createRxJSExternals(),
    // other externals here
  }
};
```
