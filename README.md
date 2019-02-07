# react-hooks-interval

[![NPM version][npm-image]][npm-url]
[![npm download][download-image]][download-url]
[![Build Status][travis-image]][travis-url]

Custom React Hooks for setInterval

## Install

>**Note:** Make sure that you have installed the correct version of `react(>= v16.8.0)` and `react-dom(>= v16.8.0)`.

### npm

```bash
npm install --save @use-hooks/interval
```

### yarn

```bash
yarn add @use-hooks/interval
```

## API

### Params

```js
/**
 * Params
 * @param {function} callback - Custom logic function
 * @param {number|null} delay - Delayed millisecond, stop if null
 */
```

### Returns

```js
/**
 * Returns
 */
```

## Usage

```js
import React, { useState } from 'react';

import useInterval from '@use-hooks/interval';

export default function App() {
  const [count, setCount] = useState(0);

  useInterval(() => {
    setCount(count + 1);
  }, 1000);

  return (
    <div>
      <h2>DEMO of <span style={{ color: '#F44336' }}>@use-hooks/interval</span></h2>
      <p>Count: {count}s</p>
    </div>
  );
}

```

[Live Show](https://use-hooks.github.io/react-hooks-interval/)

## Development

> Node >= v8 LTS

 - Clone the project to local disk
 - `npm install`
 - `npm start`

## License

MIT

> Generated by [create-react-hooks](https://github.com/use-hooks/create-react-hooks).

 [npm-image]: https://img.shields.io/npm/v/@use-hooks/interval.svg?style=flat-square
 [npm-url]: https://npmjs.org/package/@use-hooks/interval
 [download-image]: https://img.shields.io/npm/dm/@use-hooks/interval.svg?style=flat-square
 [download-url]: https://npmjs.org/package/@use-hooks/interval
 [travis-url]: https://travis-ci.org/use-hooks/react-hooks-interval
 [travis-image]: https://img.shields.io/travis/use-hooks/react-hooks-interval.svg?style=flat-square