# AlgoSortedUnion
A function that takes two or more arrays and returns a new array of unique values in the order of the original provided arrays.  In other words, all values present from all arrays should be included in their original order, but with no duplicates in the final array.  The unique numbers should be sorted by their original order, but the final array should not be sorted in numerical order.
```javascript
function uniteUnique(arr) {

   var newArray=[];
    for (var i=0; i<arguments.length; i++){
       var mapi=arguments[i].map(function(num) {
   if (!newArray.includes(num)){
        return newArray.push(num);
   }
  
});
       
    }
  return newArray ;
}

console.log(uniteUnique([1, 2, 3], [5, 2, 1]));

```
