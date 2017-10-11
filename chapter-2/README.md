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