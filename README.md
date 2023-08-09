# fullstackopen_module_2.a

first of all. you can console.log in 2 ways. 

1) console.log('props value is ' + props)

2) console.log('props value is ', props)

## javascript arrays ##

using programming operators of the JavaScript array: find, filter, and map

1) higher order functions liek filter and map, reject --> turning a list into something eslse.
   e.g. array of animals --> map  -->array of animal names
   e.g. array of naimals --> filter(turning an array into a smaller array) --> array of dogs
   e.g. array of animals --> find --> single item Fluffy the rabbit 
3) reduce basics.
   Reduce = special = super list transformation tool 

METHOD 1: 

```
   car orders = {
   { amount: 250},
   { amount: 450},
   { amount: 100},
   { amount: 200}
   }

   var totalAmt = 0
   for (var i = 0; i< orders.length; i++){
   totalAmt += orders[i].amount
   }

   console.log(totalAmt)

```



METHOD 2: using reduce 
 ```
var totalAmt = orders.reduce(function(sum, order){
return sum + order.amount 
}, 0)
```
 
OR 
``
var totalAmt = orders.reduce((sum, order) => sum + order.amount, 0)

``
   
