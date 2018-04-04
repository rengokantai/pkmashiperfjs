# pkmashiperfjs
### Loops
#### How loops affect performance
bad
```
console.time("process time")

console.time("start");
for(var i=0;i<=1000;i++){
	var ptag = document.createElement("p");
	ptag.innerText =i;
	document.body.appendChild(ptag);
}
console.timeEnd("process time");```
```

good
```
console.time("process time")
var i, ptag;
console.time("start");
for(i=0;i<=1000;i++){
	ptag = document.createElement("p");
	ptag.innerText = i;
	document.body.appendChild(ptag);
}
console.timeEnd("process time");
```



### Timers
#### What are timers and how do they affect performance?


##### Working around single-threading
callback 
- A callback method is simply a JavaScript function that's triggered when  a function is completed


## 6. Constructors, Prototypes, and Arrays
### Building with constructors and instance functions

### Understanding instances
new
- Every variable saved with that object is given a memory count of one but, if it's in an object we declare with the ```new``` keyword, that count is only
counted once rather than reused for every occurences

#### Creating instances with 'new'







