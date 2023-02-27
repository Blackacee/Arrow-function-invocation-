# Arrow-function-invocation-
 
var globalThis = this; //"window" in a browser, or "global" in Node.js
var foo = (() => this); 
console.log(foo() === globalThis); //true
var obj = { name: "Foo" };
console.log(foo.call(obj) === globalThis); //true
