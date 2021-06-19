# Immutable

- Official Doc(4.x): https://immutable-js.com/docs/#/

## Concepts and Key ides

- Functional programming -> pure function
- Immutable data cannot be changed once created
- As a performance optimization Immutable.js attempts to return the existing collection when an operation would result in an identical collection

```ts
const { Map } = require('immubtable')
const map1 = Map({ a: 1, b: 2 })
const map2 = map1.set('b', 2)
```
