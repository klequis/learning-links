
**Inserting a value at the end of an array**
````js
function removeWithSpread(list,index){
 return [...list.slice(0,index),...list.slice(index+1)];
}
````

**Inserting a value at a specified index**
````js
function insertAtIndexWithSpread(list,value,index){
 return [...list.slice(0,index),value,...list.slice(index)];
}
````

**Adding a new key-value**
````js
function addToObjectWithSpread(obj, key, value) {
 return {...obj,
  key: value,
 }
}
````