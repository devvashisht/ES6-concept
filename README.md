# ES6-concept

```
 -  on the fly compile (dynamic interpreted programming)
 - weakly typed programming langualge
 -  run in browser environment or browser sand box
 -

```

### script import

- `defer` :downlaod but execute after html download <dcript= src= ".js" defer> this is better than async as avoid crash
- '`async` : download & execute

- directly change in browser code and save it

**this** keyword : - for non-arrow fn : `this` contain object which has triggered it,it could be window object if called globally, button object if click handler , and for obj.funcction() will be object - for arrow function: value of `this` in outside or parent function as arrrow function does not have it own this.

**Closure** - every function has closure - inner function or object can access the value of outside or parent function after parent function is executed.

## Loop

- **forOf** loop only avaialble for array(`terable`) and not avaialble for `object`
- object array - for of : for (const element of elementArray) { element}
- object, array - for in : for ( const key in logEntry) { logEntry[key] }

## error Handling

- catch block for : gracefully closing or providing fallback to continue application
- throw error: throw (object, string, number)
- try{ where error could be throw} catch(error){ }
- finally : always execute no matter if there was an error or not

## weird part

- `ES` Ecma script : ecma is specification
- `es5 vs es6` : es5 older and es6 is modern javascript
- es5 is suppoerted in all browser
- es6 support by modern browser and can be transpiled to es5
- `var` function and global scopt -`let` block scope { block}

** Hoisting ** `var` variable declaration moved to the top on js code scanning where `let` does not do it and will be an error.

- with `use strict` on, var missing will be an error , reserve keyword
- `function vs method` function associated to object are method
- **Function are Object** : typeof fuctionname is = fucntion
- **function express** fuction assigned to variable
- `Default arguement` : functino(choic, defaultChoice= 20) {...}
- `Rest Parameter` :fn sum (a,b,...number){} ; sum(1,2,3,4,5,6)
- `fn inside fn` :

- `bind: future execution` fn.bind(object, params1, parmas2
- `fn bind` fn(30) : first two argument will be param1 and param2 adn third will be 30. object is only for binding context
- `call and apply : current execution` :

# DOM

- document : # document : javascript object (body,html,head,...)
- window : browser object :(document,console, alert,prompt,location,localstorage,height,width)
- element node and text node
- querySelector('css selector'),getElementById(): one element, querySelectionAll(), getElementByTagName
- nodes and element : all elmnet are nodes ,
- `attribute and properties` :
- nodelist.children : only elment node whereas nodelist.childnoes also includes textnode-
- childNodes, parentNode, parentElement
- previoussibling,nextsibling

# Object

- for of loop only on array object (iterable)
- ['key'] or [key] without '' key string it would be variable
- object/array.foreach((item)=>{})
- `spread` : person = {...person1,age:29} :shallow copy : same key will override
- property existence in object : 'info' in movies
- `this` without strict window and under `strict` will be undefined if no object context found

`Arrow fucuntion` **this** is same as it is outside arrow functino this value.

- `normal function` **this** is object which trigger fuctino

# Array : **Iterable** for-of loop

-

- array like object - are iterable (length & index) string and nodelist
- Array.of(1,2) :
- array.from(iterable) : iterable to array : for examaple "string" > [s,t,r,i,n,g]
- **unshift** add item in the beginging array.unshift("addthisatbegining") : and shift right
- **shift** array.shift() -remove first element and shift left
- **splice(startindex,noofitemtodelelte, ...item to be added)**
- `**slice(start,endindex)** : array.slice() : copy new array
- **concat**: array.concat(array2) -**indexof** : -1 if not found
  **find and findIndex** : array.find( ()=>{}):boolean ; return match object
- **include** boolean

- **Map** : key-valye: key could be of any type, duplicate is not allowed,key based access

- **Set** : no duplicate ,no index based access
- `MAP Vs Object` :

-`weak set and map` : better garbage collecton but limited operaton (only object)

- `prot0 prototypr` : **proto** on every object, prototype not on every obejct, exist only on functino object;

- prototype uses for builing object as it contain constuctor and proto is fallback object

## Event

- local storage: local stoagre stay unleass user clears it
- session storage : tab cahgnes Session stoage clear
- cookie : can be set by server, `httponly` cookie can not be acessed via client code/js

# PERFORMANCE:

- `Function execution time` can be chect using :
  >

```javascript
console.time("someFunction");
someFunction(); // Whatever is timed goes between the two "console.time"
console.timeEnd("someFunction");
```

>
