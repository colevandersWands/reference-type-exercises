# Array Exercises

* [complete the assertions 1](#complete-the-assertions 1)
* [complete the assertions 2](#complete-the-assertions 2)
* [fill in the blanks](#fill-in-the-blanks)

---

## Complete the Assertions 1

[on pytut](http://www.pythontutor.com/javascript.html#code=let%20a_1%20%3D%20%5B%5D%3B%0Alet%20a_2%20%3D%20a_1%3B%0Aconsole.assert%28a_1%20/*%20%3D%3D%3D%20or%20!%3D%3D%20%3F%20*/%20a_2%29%3B%0A%0Alet%20b_1%20%3D%20%5B%5D%3B%0Alet%20b_2%20%3D%20%5B%5D%3B%0Aconsole.assert%28b_1%20/*%20%3D%3D%3D%20or%20!%3D%3D%20%3F%20*/%20b_2%29%3B%0A%0A//%20---%0A%0A%20a_1.push%283%29%3B%0A%20a_2.push%283%29%3B%0Aconsole.assert%28a_1%20/*%20%3D%3D%3D%20or%20!%3D%3D%20%3F%20*/%20a_2%29%3B%0A%0A%20b_1.push%285%29%3B%0A%20b_2.push%285%29%3B%0Aconsole.assert%28b_1%20/*%20%3D%3D%3D%20or%20!%3D%3D%20%3F%20*/%20b_2%29%3B%0A%0A&mode=edit&origin=opt-frontend.js&py=js&rawInputLstJSON=%5B%5D)
```js
{
  let a_1 = [];
  let a_2 = a_1;
  console.assert(a_1 /* === or !== ? */ a_2);

  let b_1 = [];
  let b_2 = [];
  console.assert(b_1 /* === or !== ? */ b_2);

  // ---

  a_1.push(3);
  a_2.push(3);
  console.assert(a_1 /* === or !== ? */ a_2);

  b_1.push(5);
  b_2.push(5);
  console.assert(b_1 /* === or !== ? */ b_2);
}
```

[TOP](#array-exercises)

---

## Complete the Assertions 2

[on pytut](http://www.pythontutor.com/javascript.html#code=let%20a_1%20%3D%20%5B%5D%3B%0Alet%20a_2%20%3D%20a_1%3B%0Aconsole.assert%28a_1%20/*%20%3D%3D%3D%20or%20!%3D%3D%20%3F%20*/%20a_2%29%3B%0A%0Alet%20b_1%20%3D%20%5B%5D%3B%0Alet%20b_2%20%3D%20%5B%5D%3B%0Aconsole.assert%28b_1%20/*%20%3D%3D%3D%20or%20!%3D%3D%20%3F%20*/%20b_2%29%3B%0A%0A//%20---%0A%0Aconst%20key%20%3D%200%3B%0A%0A%20a_1%5Bkey%5D%20%3D%203%3B%0A%20a_2%5Bkey%5D%20%3D%203%3B%0Aconsole.assert%28a_1%20/*%20%3D%3D%3D%20or%20!%3D%3D%20%3F%20*/%20a_2%29%3B%0A%0A%20b_1%5Bkey%5D%20%3D%205%3B%0A%20b_2%5Bkey%5D%20%3D%205%3B%0Aconsole.assert%28b_1%20/*%20%3D%3D%3D%20or%20!%3D%3D%20%3F%20*/%20b_2%29%3B%0A&mode=edit&origin=opt-frontend.js&py=js&rawInputLstJSON=%5B%5D)
```js
{
  let a_1 = [];
  let a_2 = a_1;
  console.assert(a_1 /* === or !== ? */ a_2);

  let b_1 = [];
  let b_2 = [];
  console.assert(b_1 /* === or !== ? */ b_2);

  // ---

  const index = 0;

  a_1[index] = 3;
  a_2[index] = 3;
  console.assert(a_1 /* === or !== ? */ a_2);

  b_1[index] = 5;
  b_2[index] = 5;
  console.assert(b_1 /* === or !== ? */ b_2);
}
```

[TOP](#array-exercises)

---

## Fill in the Blanks

[on pytut](http://www.pythontutor.com/live.html#code=%20%20%20%20%3B%20//%20write%20this%20line%0A%20%20%20%20%3B%20//%20write%20this%20line%0Aconsole.assert%28arr_1%20!%3D%3D%20arr_2%29%3B%0Aconsole.assert%28arr_1%5B1%5D%20%3D%3D%3D%20arr_2%5B1%5D%29%3B%0Aconsole.assert%28arr_1%5B1%5D%20%3D%3D%3D%20'B'%29%0A%0Alet%20key%20%3D%200%3B%0Aconsole.assert%28arr_1%5Bkey%5D%20%3D%3D%3D%20arr_2%5Bkey%5D%29%3B%0Aconsole.assert%28arr_1%5Bkey%5D%20%3D%3D%3D%20'A'%29%3B%0A%0A%20%20%20%20%3B%20//%20write%20this%20line%0A%20%20%20%20%3B%20//%20write%20this%20line%0Aconsole.assert%28arr_1%5Barr_2%5B2%5D%5D%20%3D%3D%3D%20arr_2%5Barr_1%5B2%5D%5D%29%3B%0Aconsole.assert%28arr_1%5Barr_2%5B2%5D%5D%20%3D%3D%3D%20'B'%29%3B%0A%0A%20%20%20%20%3B%20//%20write%20this%20line%0A%20%20%20%20%3B%20//%20write%20this%20line%0Aconsole.assert%28arr_1%20%3D%3D%3D%20arr_2%29%3B%0Aconsole.assert%28arr_3%20!%3D%3D%20arr_1%29%3B%0Aconsole.assert%28arr_3%20!%3D%3D%20arr_2%29%3B%0Aconsole.assert%28arr_3%5Bkey%5D%20%3D%3D%3D%20arr_1%5B0%5D%29%3B%0A%0A%20%20%20%20%3B%20//%20write%20this%20line%0Aconsole.assert%28obj_3%5B1%5D%20%3D%3D%3D%20obj_2%5Bkey%5D%29%3B&cumulative=false&curInstr=1&heapPrimitives=nevernest&mode=display&origin=opt-live.js&py=js&rawInputLstJSON=%5B%5D&textReferences=false)
```js
{
      ; // write this line
      ; // write this line
  console.assert(arr_1 !== arr_2);
  console.assert(arr_1[1] === arr_2[1]);
  console.assert(arr_1[1] === 'B')

  let key = 0;
  console.assert(arr_1[key] === arr_2[key]);
  console.assert(arr_1[key] === 'A');

      ; // write this line
      ; // write this line
  console.assert(arr_1[arr_2[2]] === arr_2[arr_1[2]]);
  console.assert(arr_1[arr_2[2]] === 'B');

      ; // write this line
      ; // write this line
  console.assert(arr_1 === arr_2);
  console.assert(arr_3 !== arr_1);
  console.assert(arr_3 !== arr_2);
  console.assert(arr_3[key] === arr_1[0]);

      ; // write this line
  console.assert(obj_3[1] === obj_2[key]);
}
```

[TOP](#array-exercises)

___
___
### <a href="http://janke-learning.org" target="_blank"><img src="https://user-images.githubusercontent.com/18554853/50098409-22575780-021c-11e9-99e1-962787adaded.png" width="40" height="40"></img> Janke Learning</a>
