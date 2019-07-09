# Object Exercises

* [complete the assertions 1](#complete-the-assertions 1)
* [complete the assertions 2](#complete-the-assertions 2)
* [fill in the blanks](#fill-in-the-blanks)

---

## Complete the Assertions 1

[on pytut](http://www.pythontutor.com/javascript.html#code=let%20a_1%20%3D%20%7B%7D%3B%0Alet%20a_2%20%3D%20a_1%3B%0Aconsole.assert%28a_1%20/*%20%3D%3D%3D%20or%20!%3D%3D%20%3F%20*/%20a_2%29%3B%0A%0Alet%20b_1%20%3D%20%7B%7D%3B%0Alet%20b_2%20%3D%20%7B%7D%3B%0Aconsole.assert%28b_1%20/*%20%3D%3D%3D%20or%20!%3D%3D%20%3F%20*/%20b_2%29%3B%0A%0A//%20---%0A%0Alet%20a_1.x%20%3D%203%3B%0Alet%20a_2.x%20%3D%203%3B%0Aconsole.assert%28a_1%20/*%20%3D%3D%3D%20or%20!%3D%3D%20%3F%20*/%20a_2%29%3B%0A%0Alet%20b_1.x%20%3D%205%3B%0Alet%20b_2.x%20%3D%205%3B%0Aconsole.assert%28b_1%20/*%20%3D%3D%3D%20or%20!%3D%3D%20%3F%20*/%20b_2%29%3B%0A%0A&mode=edit&origin=opt-frontend.js&py=js&rawInputLstJSON=%5B%5D)
```js
{
  let a_1 = {};
  let a_2 = a_1;
  console.assert(a_1 /* === or !== ? */ a_2);

  let b_1 = {};
  let b_2 = {};
  console.assert(b_1 /* === or !== ? */ b_2);

  // ---

  let a_1.x = 3;
  let a_2.x = 3;
  console.assert(a_1 /* === or !== ? */ a_2);

  let b_1.x = 5;
  let b_2.x = 5;
  console.assert(b_1 /* === or !== ? */ b_2);
}
```

[TOP](#object-exercises)

---

## Complete the Assertions 2

[on pytut](http://www.pythontutor.com/javascript.html#code=%20%20let%20a_1%20%3D%20%7B%7D%3B%0A%20%20let%20a_2%20%3D%20a_1%3B%0A%20%20console.assert%28a_1%20/*%20%3D%3D%3D%20or%20!%3D%3D%20%3F%20*/%20a_2%29%3B%0A%0A%20%20let%20b_1%20%3D%20%7B%7D%3B%0A%20%20let%20b_2%20%3D%20%7B%7D%3B%0A%20%20console.assert%28b_1%20/*%20%3D%3D%3D%20or%20!%3D%3D%20%3F%20*/%20b_2%29%3B%0A%0A%20%20//%20---%0A%20%20%0A%20%20const%20key%20%3D%20%22x%22%3B%0A%0A%20%20let%20a_1%5Bkey%5D%20%3D%203%3B%0A%20%20let%20a_2%5Bkey%5D%20%3D%203%3B%0A%20%20console.assert%28a_1%20/*%20%3D%3D%3D%20or%20!%3D%3D%20%3F%20*/%20a_2%29%3B%0A%0A%20%20let%20b_1%5Bkey%5D%20%3D%205%3B%0A%20%20let%20b_2%5Bkey%5D%20%3D%205%3B%0A%20%20console.assert%28b_1%20/*%20%3D%3D%3D%20or%20!%3D%3D%20%3F%20*/%20b_2%29%3B&mode=edit&origin=opt-frontend.js&py=js&rawInputLstJSON=%5B%5D)
```js
{
  let a_1 = {};
  let a_2 = a_1;
  console.assert(a_1 /* === or !== ? */ a_2);

  let b_1 = {};
  let b_2 = {};
  console.assert(b_1 /* === or !== ? */ b_2);

  // ---

  const key = "x";

  let a_1[key] = 3;
  let a_2[key] = 3;
  console.assert(a_1 /* === or !== ? */ a_2);

  let b_1[key] = 5;
  let b_2[key] = 5;
  console.assert(b_1 /* === or !== ? */ b_2);
}
```

[TOP](#object-exercises)

---

## Fill in the Blanks

[on pytut](http://www.pythontutor.com/live.html#code=%20%20%20%20%3B%20//%20write%20this%20line%0A%20%20%20%20%3B%20//%20write%20this%20line%0Aconsole.assert%28obj_1%20!%3D%3D%20obj_2%29%3B%0Aconsole.assert%28obj_1.x%20%3D%3D%3D%20obj_2.x%29%3B%0A%0Alet%20key%20%3D%20%22y%22%3B%0Aconsole.assert%28obj_1%5Bkey%5D%20%3D%3D%3D%20obj_2%5Bkey%5D%29%3B%0A%0A%20%20%20%20%3B%20//%20write%20this%20line%0A%20%20%20%20%3B%20//%20write%20this%20line%0Aconsole.assert%28obj_1%5Bobj_2.y%5D%20%3D%3D%3D%20obj_2%5Bobj_1.y%5D%29%3B%0Aconsole.assert%28obj_1%5Bobj_2.y%5D%20%3D%3D%3D%20obj_1%5B'x'%5D%29%3B%0A%0A%20%20%20%20%3B%20//%20write%20this%20line%0A%20%20%20%20%3B%20//%20write%20this%20line%0Aconsole.assert%28obj_1%20%3D%3D%3D%20obj_2%29%3B%0Aconsole.assert%28obj_3%20!%3D%3D%20obj_1%29%3B%0Aconsole.assert%28obj_3%20!%3D%3D%20obj_2%29%3B%0Aconsole.assert%28obj_3%5Bkey%5D%20%3D%3D%3D%20obj_1.y%29%3B%0A%0A%20%20%20%20%3B%20//%20write%20this%20line%0Aconsole.assert%28obj_3.x%20%3D%3D%3D%20obj_2%5Bkey%5D%29%3B&cumulative=false&curInstr=1&heapPrimitives=nevernest&mode=display&origin=opt-live.js&py=js&rawInputLstJSON=%5B%5D&textReferences=false)
```js
{
      ; // write this line
      ; // write this line
  console.assert(obj_1 !== obj_2);
  console.assert(obj_1.x === obj_2.x);

  let key = "y";
  console.assert(obj_1[key] === obj_2[key]);

      ; // write this line
      ; // write this line
  console.assert(obj_1[obj_2.y] === obj_2[obj_1.y]);
  console.assert(obj_1[obj_2.y] === obj_1['x']);

      ; // write this line
      ; // write this line
  console.assert(obj_1 === obj_2);
  console.assert(obj_3 !== obj_1);
  console.assert(obj_3 !== obj_2);
  console.assert(obj_3[key] === obj_1.y);

      ; // write this line
  console.assert(obj_3.x === obj_2[key]);
}
```

[TOP](#object-exercises)


___
___
### <a href="http://janke-learning.org" target="_blank"><img src="https://user-images.githubusercontent.com/18554853/50098409-22575780-021c-11e9-99e1-962787adaded.png" width="40" height="40"></img> Janke Learning</a>
