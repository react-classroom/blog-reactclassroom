---
layout: post
title: "Iterables en ES6"
date: 2019-01-28
categories: ecmascript
author: carlosrojas
tags: [ecmascript]
cover: "https://firebasestorage.googleapis.com/v0/b/vueclassroom.appspot.com/o/2018-12-27-intro-es6%2Fecmascript.png?alt=media&token=335db467-ce9e-4e06-9a2d-fc86a785df0b"
editname: '2019-01-28-Iterables-Looping.md'
versions:
  - title: 'EcmaScript'
    number: '6'
---

> Existe ocasiones en las que obtenemos `Objetos` y/o `Arrays` de los cuales queremos independizar su contenido en distintas variables las cuales queremos utilizar en diferentes calculos, esto resulta facil cuando tenemos 1 o 2 datos pero cuando son muchos este proceso se vuelve muy engorroso.

<amp-img width="1024" height="450" layout="responsive" src="https://firebasestorage.googleapis.com/v0/b/vueclassroom.appspot.com/o/2018-12-27-intro-es6%2Fecmascript.png?alt=media&token=335db467-ce9e-4e06-9a2d-fc86a785df0b"></amp-img>

{% include general/net-promoter-score.html %} 


```js
const data = ['item1', 'item2', 'item3', 'item 4'];

data.forEach(
  (item)=> {
    console.log(item);
  }
)
```

```js
const data = ['item1', 'item2', 'item3', 'item 4'];

for(let i=0; i < data.length; i++) {
  console.log(data[i]);
}
```

```js
const data = ['item1', 'item2', 'item3', 'item 4'];

for(const index in data) {
  console.log(data[index]);
}
```

```js
const data = ['item1', 'item2', 'item3', 'item 4'];

for(const item of data) {
  console.log(data);
}
```

```js
const data = ['item1', 'item2', 'item3', 'item 4'];

for(const [i, item] of data.entries()) {
  console.log("Posicion: " + i);
  console.log("Item: " + item);
}
```

```js
const data = {
  prop1: 'item1', 
  prop2: 'item2', 
  prop3: 'item3', 
  prop4: 'item 4'
};

for(const prop of  Object.keys[data]) {
  const value = data[prop];
  console.log("Posicion: " + i);
  console.log("Item: " + item);
}
```

```js
const data = {
  prop1: 'item1', 
  prop2: 'item2', 
  prop3: 'item3', 
  prop4: 'item 4'
};

for(const prop in data) {
  const value = data[prop];
  console.log("Posicion: " + i);
  console.log("Item: " + item);
}
```
