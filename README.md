# react-numscroll
A React Component for Counting Numbers
### npm https://www.npmjs.com/package/react-numscroll


# React Number Scrolling

### Install

`npm install react-numscroll`
or
`yarn add react-numscroll`

### **Quickstart**

```js
import React, { useState, useEffect } from 'react';
import NumberScroll from 'react-numscroll';

export default () => {
  const [count, setCount] = useState(10);

  useEffect(() => {
    setInterval(() => {
      setCount(count => ++count);
    }, 2000);
  }, []);

  return <NumberScroll number={count} itemWidth={50} itemHeight={60} />;
};
```

### **API**

| Prop         | Type   | Required | Description                                          |
| ------------ | ------ | -------- | ---------------------------------------------------- |
| `number`     | number | Yes      | what does number come in                             |
| `itemWidth`  | number | No       | Individual number width.<br />Default: 50            |
| `itemHeight` | number | No       | Individual number height.<br />Default: 60           |
| `numSize`    | number | No       | Individual number size. Default: 32                  |
| `numColor`   | string | No       | Number color. <br />Default: #fff                    |
| `bgColor`    | string | No       | Background color<br />Default:#0089e9                |
| `border`     | string | No       | Individual number border. Default: 1px solid #f9f9f9 |
