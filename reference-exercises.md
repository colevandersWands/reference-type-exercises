# Reference Exercises

* [swap object and array](#swap-object-and-array)
* [complete this code](#complete-this-code)


---

## Swap Object and Array

[on pytut](http://www.pythontutor.com/javascript.html#code=let%20obj%20%3D%20%5B%5D%3B%0Alet%20arr%20%3D%20%7B%7D%3B%0Alet%20_%20%3D%20null%3B%0A%0A//%20swap%20the%20object%20and%20the%20array&mode=edit&origin=opt-frontend.js&py=js&rawInputLstJSON=%5B%5D)
```js
{
  let obj = [];
  let arr = {};
  let _ = null;

  // --- swap here ---



  // --- asserts ---

  const obj_strified = JSON.stringify(obj);
  console.assert(obj_strified === "{}", "obj is bad");

  const arr_strified = JSON.stringify(arr);
  console.assert(arr_strified === "[]", "arr is bad");
}
```


[TOP](#reference-exercises)

---

## Complete this code

([read this first](https://github.com/janke-learning/reference-vs-value))  
[on pytut](http://www.pythontutor.com/live.html#code=%20%20let%20value_1%20%3D%205%3B%0A%20%20let%20reference_1%20%3D%20%5B%5D%3B%0A%0A%20%20let%20value_2%20%3D%20value_1%3B%0A%20%20console.assert%28value_2%20/*%20%3D%3D%3D%20or%20!%3D%3D%20%3F%20*/%20value_1,%20%22assert%201%22%29%3B%0A%0A%20%20let%20reference_2%20%3D%20reference_1%3B%0A%20%20console.assert%28reference_2%20/*%20%3D%3D%3D%20or%20!%3D%3D%20%3F%20*/%20reference_1,%20%22assert%202%22%29%3B%0A%0A%20%20%3B%20//%20write%20this%20line%0A%20%20console.assert%28value_1%20!%3D%3D%20value_2,%20%22assert%203%22%29%3B%20%20%0A%0A%20%20%3B%20//%20write%20this%20line%0A%20%20console.assert%28reference_1%5B0%5D%20%3D%3D%3D%20reference_2%5B0%5D,%20%22assert%204%22%29%3B%0A%0A%20%20%3B%20//%20write%20this%20line%0A%20%20console.assert%28reference_1%20%3D%3D%3D%20reference_2,%20%22assert%205%22%29%3B%0A%0A%20%20//%20remove%20the%20array%20from%20memory%0A%20%20%3B%20//%20write%20this%20line%0A%20%20%3B%20//%20write%20this%20line&cumulative=false&heapPrimitives=nevernest&mode=display&origin=opt-live.js&py=js&rawInputLstJSON=%5B%5D&textReferences=false)
```js
{
  let value_1 = 5;
  let reference_1 = [];

  let value_2 = value_1;
  console.assert(value_2 /* === or !== ? */ value_1, "assert 1");

  let reference_2 = reference_1;
  console.assert(reference_2 /* === or !== ? */ reference_1, "assert 2");

  ; // write this line
  console.assert(value_1 !== value_2, "assert 3");  

  ; // write this line
  console.assert(reference_1[0] === reference_2[0], "assert 4");

  ; // write this line
  console.assert(reference_1 === reference_2, "assert 5");

  // remove the array from memory
  ; // write this line
  ; // write this line
}
```

[TOP](#reference-exercises)

___
___
### <a href="http://janke-learning.org" target="_blank"><img src="https://user-images.githubusercontent.com/18554853/50098409-22575780-021c-11e9-99e1-962787adaded.png" width="40" height="40"></img> Janke Learning</a>

