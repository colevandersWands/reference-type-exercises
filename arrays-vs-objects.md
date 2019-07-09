# Arrays vs Objects

* [swap them 1](#swap-them-1)
* [swap them 2](#swap-them-2)
* [relative vs. absolute](#relative-vs-absolute)

---

## Swap them 1

[on pytut](http://www.pythontutor.com/javascript.html#code=const%20obj%20%3D%20%7Bprop%3A%20%22array%22%7D%3B%0Aconst%20arr%20%3D%20%5B%22object%22%5D%3B%0Alet%20_%20%3D%20null%3B%0A%0A//%20swap%20the%20values%20stored%20in%20each%20structure%0A//%20%20using%20dot%20notation%20for%20the%20object%0A//%20%20using%20direct%20access%20for%20the%20array&mode=edit&origin=opt-frontend.js&py=js&rawInputLstJSON=%5B%5D)
```js
{
  const obj = {prop: "array"};
  const arr = ["object"];
  let _ = null;

  // swap the values stored in each structure


  // asserts
  console.assert(obj.prop === "object", "obj assert");
  console.assert(arr[0] === "array", "arr assert");
}
```


[TOP](#objects-vs-arrays)

---

## Swap them 2

[on pytut](http://www.pythontutor.com/javascript.html#code=const%20obj%20%3D%20%7Bprop%3A%20%22array%22%7D%3B%0Aconst%20arr%20%3D%20%5B%22object%22%5D%3B%0Alet%20_%20%3D%20null%3B%0A%0A//%20swap%20the%20values%20stored%20in%20each%20structure%0A//%20%20using%20bracket%20notation%20for%20the%20object%0A//%20%20using%20variable%20access%20for%20the%20array%0Aconst%20obj_key%20%3D%20%3B%0Aconst%20arr_index%20%3D%20%3B&mode=edit&origin=opt-frontend.js&py=js&rawInputLstJSON=%5B%5D)  
```js
{
  const obj = {prop: "array"};
  const arr = ["object"];
  let _ = null;

  // swap the values stored in each structure
  const obj_key = ;
  const arr_index = ;


  // asserts
  console.assert(obj[obj_key] === "object", "obj assert");
  console.assert(arr[arr_index] === "array", "arr assert");
}
```

[TOP](#objects-vs-arrays)

---

## Relative vs Absolute

[on pytut](http://www.pythontutor.com/javascript.html#code=//%20array%20indices%20are%20relative%0Aconst%20arr%20%3D%20%5B%22a%22,%20%22b%22%5D%3B%0Aconst%20index%20%3D%200%3B%0A%0Aconst%20read_arr_1%20%3D%20arr%5Bindex%5D%3B%0Aarr.shift%28%29%3B%20//%20removes%20the%20first%20item%0Aconst%20read_arr_2%20%3D%20arr%5Bindex%5D%3B%0A%0Aconsole.assert%28read_arr_1%20/*%20%3D%3D%3D%20or%20!%3D%3D%20%3F%20*/%20read_arr_2%29%3B%0A%0A//%20object%20keys%20are%20absolute%0Aconst%20obj%20%3D%20%7Bx%3A%20%22a%22,%20y%3A%20%22b%22%7D%3B%0Aconst%20key%20%3D%20%22y%22%3B%0A%0Aconst%20read_obj_1%20%3D%20obj%5Bkey%5D%3B%0Adelete%20obj.x%3B%0Aconst%20read_obj_2%20%3D%20obj%5Bkey%5D%3B%0A%0Aconsole.assert%28read_obj_1%20/*%20%3D%3D%3D%20or%20!%3D%3D%20%3F%20*/%20read_obj_2%29%3B&mode=edit&origin=opt-frontend.js&py=js&rawInputLstJSON=%5B%5D)  
```js
{
  // array indices are relative
  const arr = ["a", "b"];
  const index = 0;

  const read_arr_1 = arr[index];
  arr.shift(); // removes the first item
  const read_arr_2 = arr[index];

  console.assert(read_arr_1 /* === or !== ? */ read_arr_2);

  // object keys are absolute
  const obj = {x: "a", y: "b"};
  const key = "y";

  const read_obj_1 = obj[key];
  delete obj.x;
  const read_obj_2 = obj[key];

  console.assert(read_obj_1 /* === or !== ? */ read_obj_2);
}
```

[TOP](#objects-vs-arrays)

___
___
### <a href="http://janke-learning.org" target="_blank"><img src="https://user-images.githubusercontent.com/18554853/50098409-22575780-021c-11e9-99e1-962787adaded.png" width="40" height="40"></img> Janke Learning</a>
