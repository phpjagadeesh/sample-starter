# Conceptual Aside

## Here we have three important concepts 

### Syntax Parser
The syntax parser is translate human readable code to computer instruction through interpreter or compailer.


### Lexical Enviorment
The Lexical enviorment means where the code is actually sitting

```javascript
function hello() {
    var a = 0;
}
```

Here variable *a* is lexically inside the function *hello*


### Execution Context
The Execution context is, which once is currently exicuting managed by exicution context.   



## Name-Value pairs
The 'value' which map to name. The value it self another name-value pairs.

```javascript
address: {
    first: 'This',
    age: 20,
    street: {
      address1: 'test',
      address2: 'test2'
    }
}

``` 

## Global object 
When execution statrted the javascript engine automatically create two things
1. Global Object
2. Special variable 'this' 

There is always a global object. Lexically your code not sitting inside a function then that code 'global'

```javascript
var a = 'hello javascript';
console.log(a);
console.log(window.a);
```
In the above code both 'a' and 'window.a' will work because 'a' is attached to global object. if the code running inside a function then there is 'outer enviroment'.


## Hoisting
Before move to hoisting, when code statrted to exicute then two phase will face
1. Creation part
2. Exicution part

When the cretation part all variables and functions are place inside memory space. In the exicution part all these code will invoke

```javascript
a('jagadeesh');

function a(name) {
  console.log('my name is' + name);    
}
```
The function a() is called before declarion but it will work fine reason is, In the creation phase all function will placed in memory space first.
