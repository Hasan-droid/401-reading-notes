## Array.map()

The `map()` method creates a new array populated with the results of calling a provided function on every element in the calling array.  

&nbsp;
## Array.reduce()  

The `reduce()` method executes a reducer function (that you provide) on each element of the array, resulting in a single output value.  
&nbsp;
## superagent()
&nbsp;
* With normal Promise `.then()` syntax

```
superagent.get('url')
 .then(res => {
      alert('yay got ' + JSON.stringify(res.body));
   });
```

&nbsp;
&nbsp;

* With `async / await` syntax

```
(async () => {
>  try {
    const res = await superagent.post('/api/pet');
    console.log(res);
  } catch (err) {
    console.error(err);
  }
})();
```


&nbsp;
## Promises


The Promise object represents the eventual completion (or failure) of an asynchronous operation and its resulting value.

&nbsp;

## When callback functions considered to be Asynchronous?

For a function to be asynchronous it needs to perform an asynchronous operation. It needs to incorporate the argument callback in handling the results of this asynchronous operation. Only this way the function becomes asynchronous.