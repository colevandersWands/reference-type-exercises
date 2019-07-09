# Examples to Study


* [comparing reference types](#comparing-reference-types)
* [swapping with arrays](#swapping-with-arrays)
* swapping with objects
    * [dot notation](#dot-notation)
    * [bracket notation](#bracket-notation)

---

## Comparing Reference Types

[on pytut](http://www.pythontutor.com/live.html#code=let%20a%20%3D%20%5B%5D%3B%0Alet%20b%20%3D%20%5B%5D%3B%0Aconsole.assert%28a%20!%3D%3D%20b%29%3B%0Aconsole.assert%28a%20%3D%3D%3D%20b%29%3B%0A%0Ab%20%3D%20a%3B%0Aconsole.assert%28a%20%3D%3D%3D%20b%29%3B%0Aconsole.assert%28a%20!%3D%3D%20b%29%3B&cumulative=false&curInstr=0&heapPrimitives=nevernest&mode=display&origin=opt-live.js&py=js&rawInputLstJSON=%5B%5D&textReferences=false)  
```js
{
  let a = [];
  let b = [];
  console.assert(a !== b);
  console.assert(a === b);
  
  b = a;
  console.assert(a === b);
  console.assert(a !== b);
}
```

[TOP](#examples-to-study)

___


## Swapping with Arrays

[on pytut](http://www.pythontutor.com/javascript.html#code=let%20a%20%3D%20%5B%22b%22%5D%3B%0Alet%20b%20%3D%20%5B%22a%22%5D%3B%0Alet%20_%20%3D%20null%3B%0A%0A//%20swap%20the%20arrays%20to%20which%20each%20variable%20points%0A_%20%3D%20a%3B%0Aa%20%3D%20b%3B%0Ab%20%3D%20_%3B%0A%0A//%20------%0A%0A_%20%3D%20null%3B%0Alet%20x%20%3D%20%5B%22y%22%5D%3B%0Alet%20y%20%3D%20%5B%22x%22%5D%3B%0A%0A//%20swap%20the%20value%20each%20array%20contains%0A_%20%3D%20x%5B0%5D%3B%0Ax%5B0%5D%20%3D%20y%5B0%5D%3B%0Ay%5B0%5D%20%3D%20_%3B&curInstr=0&mode=display&origin=opt-frontend.js&py=js&rawInputLstJSON=%5B%5D)
```js
{
  let a = ["b"];
  let b = ["a"];
  let _ = null;

  // swap the arrays to which each variable points
  _ = a;
  a = b;
  b = _;

  // ------

  _ = null;
  let x = ["y"];
  let y = ["x"];

  // swap the value each array contains
  _ = x[0];
  x[0] = y[0];
  y[0] = _;
}
```


[TOP](#examples-to-study)

___


## Swapping with Objects 

### dot notation

[on pytut](http://www.pythontutor.com/javascript.html#code=let%20a%20%3D%20%7Bb_prop%3A%20%22b%22%7D%3B%0Alet%20b%20%3D%20%7Ba_prop%3A%20%22a%22%7D%3B%0Alet%20_%20%3D%20null%3B%0A%0A//%20swap%20the%20object%20in%20which%20each%20value%20is%20stored%0A_%20%3D%20a%3B%0Aa%20%3D%20b%3B%0Ab%20%3D%20_%3B%0A%0A//%20------%0A%0A_%20%3D%20null%3B%0Alet%20x%20%3D%20%7Bx_prop%3A%20%22y%22%7D%3B%0Alet%20y%20%3D%20%7By_prop%3A%20%22x%22%7D%3B%0A%0A//%20swap%20the%20value%20each%20object%20contains%0A_%20%3D%20x.x_prop%3B%0Ax.x_prop%20%3D%20y.y_prop%3B%0Ay.y_prop%20%3D%20_%3B%0A&curInstr=0&mode=display&origin=opt-frontend.js&py=js&rawInputLstJSON=%5B%5D)
```js
{
  let a = {b_prop: "b"};
  let b = {a_prop: "a"};
  let _ = null;

  // swap the object in which each value is stored
  _ = a;
  a = b;
  b = _;

  // ------

  _ = null;
  let x = {x_prop: "y"};
  let y = {y_prop: "x"};

  // swap the value each object contains
  _ = x.x_prop;
  x.x_prop = y.y_prop;
  y.y_prop = _;
}
```


### bracket notation

[(read this first)](https://github.com/janke-learning/dots-vs-brackets)  
[on pytut](http://www.pythontutor.com/javascript.html#code=let%20a%20%3D%20%7Ba_prop%3A%20%22b%22%7D%3B%0Alet%20b%20%3D%20%7Bb_prop%3A%20%22a%22%7D%3B%0Alet%20_%20%3D%20null%3B%0A%0A//%20swap%20the%20object%20in%20which%20each%20value%20is%20stored%0A//%20%20with%20dots%0A_%20%3D%20a.a_prop%3B%0Aa.a_prop%20%3D%20b.b_prop%3B%0Ab.b_prop%20%3D%20_%3B%0A%0A//%20------%0A%0A_%20%3D%20null%3B%0Alet%20x%20%3D%20%7Bx_prop%3A%20%22y%22%7D%3B%0Alet%20y%20%3D%20%7By_prop%3A%20%22x%22%7D%3B%0A%0A//%20swap%20the%20object%20in%20which%20each%20value%20is%20stored%0A//%20%20with%20brackets%0Aconst%20x_key%20%3D%20%22x_prop%22%3B%0Aconst%20y_key%20%3D%20%22y_prop%22%3B%0A_%20%3D%20x%5Bx_key%5D%3B%0Ax%5Bx_key%5D%20%3D%20y%5By_key%5D%3B%0Ay%5By_key%5D%20%3D%20_%3B%0A&curInstr=0&mode=display&origin=opt-frontend.js&py=js&rawInputLstJSON=%5B%5D)
```js
{
  let a = {a_prop: "b"};
  let b = {b_prop: "a"};
  let _ = null;

  // swap the object in which each value is stored
  //  with dots
  _ = a.a_prop;
  a.a_prop = b.b_prop;
  b.b_prop = _;

  // ------

  _ = null;
  let x = {x_prop: "y"};
  let y = {y_prop: "x"};

  // swap the object in which each value is stored
  //  with brackets
  const x_key = "x_prop";
  const y_key = "y_prop";
  _ = x[x_key];
  x[x_key] = y[y_key];
  y[y_key] = _;
}
```

[TOP](#examples-to-study)

___
___
### <a href="http://janke-learning.org" target="_blank"><img src="https://user-images.githubusercontent.com/18554853/50098409-22575780-021c-11e9-99e1-962787adaded.png" width="40" height="40"></img> Janke Learning</a>
