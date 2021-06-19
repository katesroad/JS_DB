# Immutable

- Official Doc(4.x): https://immutable-js.com/docs/#/

## Concepts and Key ides

- Functional programming -> pure function -> data-in & data-out
- Immutable data can't be changed once created
- As a performance optimization Immutable.js attempts to return the existing collection when an operation would result in an identical collection

```ts
const { Map } = require('immubtable')
const map1 = Map({ a: 1, b: 2 })
const map2 = map1.set('b', 2)
console.log(map1 === map2) // true
```

## Key APIS

- is & equals

```ts
const { Map } = require('immutable')
const map1 = Map({ a: '1', b: '2' })
const map2 = Map({ a: '1', b: '2' })

console.log(map1.equals(map2))
```
