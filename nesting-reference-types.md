# Nesting Reference Types

* arrays
    * [complete the asserts 1](#complete-the-asserts-1)
    * [fill in the blanks 1](#fill-in-the-blanks-1)
* objects
* arrays and objects

---

## complete the asserts

[on pytut](http://www.pythontutor.com/live.html#code=let%20arr_1%20%3D%20%5B%5D%3B%0Alet%20arr_2%20%3D%20%5B%5D%3B%0A%0Aarr_1.push%28arr_2%29%3B%0Aarr_2.push%28arr_1%29%3B%0Aconsole.assert%28arr_1%5B0%5D%20/*%20%3D%3D%3D%20or%20!%3D%3D%20*/%20arr_2%29%3B%0Aconsole.assert%28arr_2%5B0%5D%20/*%20%3D%3D%3D%20or%20!%3D%3D%20*/%20arr_1%29%3B%0A%0Aarr_1.push%28%5B%5D%29%3B%0Aarr_2.push%28%5B%5D%29%3B%0Aconsole.assert%28arr_1%5B1%5D%20/*%20%3D%3D%3D%20or%20!%3D%3D%20*/%20arr_2%5B1%5D%29%3B%0A%0Aarr_1%5B0%5D.push%28'A'%29%3B%0Aconsole.assert%28arr_1%5B0%5D%5B2%5D%20/*%20%3D%3D%3D%20or%20!%3D%3D%20*/%20arr_2%5B2%5D%29%3B%0A%0Aarr_2%5B0%5D.push%28'B'%29%3B%0Aconsole.assert%28arr_2%5B0%5D%5B2%5D%20/*%20%3D%3D%3D%20or%20!%3D%3D%20*/%20arr_1%5B2%5D%29%3B%0A%0Aarr_1%5B1%5D.push%28'X'%29%3B%0Aarr_2%5B1%5D.push%28'X'%29%3B%0Aconsole.assert%28arr_1%5B1%5D%5B0%5D%20/*%20%3D%3D%3D%20or%20!%3D%3D%20*/%20arr_2%5B1%5D%5B0%5D%29&cumulative=false&curInstr=9&heapPrimitives=nevernest&mode=display&origin=opt-live.js&py=js&rawInputLstJSON=%5B%5D&textReferences=false)
```js
{
  let arr_1 = [];
  let arr_2 = [];

  arr_1.push(arr_2);
  arr_2.push(arr_1);
  console.assert(arr_1[0] /* === or !== */ arr_2);
  console.assert(arr_2[0] /* === or !== */ arr_1);

  arr_1.push([]);
  arr_2.push([]);
  console.assert(arr_1[1] /* === or !== */ arr_2[1]);

  arr_1[0].push('A');
  console.assert(arr_1[0][2] /* === or !== */ arr_2[2]);
  
  arr_2[0].push('B');
  console.assert(arr_2[0][2] /* === or !== */ arr_1[2]);

  arr_1[1].push('X');
  arr_2[1].push('X');
  console.assert(arr_1[1][0] /* === or !== */ arr_2[1][0])
}
```


[TOP](#nesting-reference-types)

---

## fill in the blanks 1

```js
{
  let arr_1 = [];
  let arr_2 = [];

  arr_1.push(arr_2);
  arr_2.push(arr_1);
  console.assert(arr_1[0] /* === or !== */ arr_2);
  console.assert(arr_2[0] /* === or !== */ arr_1);

  arr_1.push([]);
  arr_2.push([]);
  console.assert(arr_1[1] /* === or !== */ arr_2[1]);

  arr_1[0].push('A');
  console.assert(arr_1[0][2] /* === or !== */ arr_2[2]);
  
  arr_2[0].push('B');
  console.assert(arr_2[0][2] /* === or !== */ arr_1[2]);

  arr_1[1].push('X');
  arr_2[1].push('X');
  console.assert(arr_1[1][0] /* === or !== */ arr_2[1][0])
}
```


[TOP](#nesting-reference-types)

---

### Nesting Objects


[TOP](#nesting-reference-types)

---

### Nesting Arrays and Objects


[TOP](#nesting-reference-types)

___
___
### <a href="http://janke-learning.org" target="_blank"><img src="https://user-images.githubusercontent.com/18554853/50098409-22575780-021c-11e9-99e1-962787adaded.png" width="40" height="40"></img> Janke Learning</a>
