To understand range , we need to start from iterables.

🟦 What are iterables ?
🟡 An iterable is a object (because every data is a object in python) which contain countable number of values and we can access each element of that object through traversing over that object one by one called as iterables. Matlab ek esa object or type of data which contains multiple elements in it together and loop ke through we can access each element of that object . Like: "Hello" is a str and a iterable as each str is a collection of characters and also we can access "H" , "e" , "l" , "l" , "o" seprately one by one through traversing .

🟢 Technically , in Python a iterable is an object which implements the iterator protocol , which consits of methods iter() and next() .


🟦 What are various types of iterables ?
🟡 range
🟡 list
🟡 tuple
🟡 str
🟡 bytes
🟡 bytearray
🟡 set
🟡 frozenset
🟡 dict



🟦 range
📀 range is a class(jaise int , bool , str etc. are class , Simliarly it is also a class) in python .
📀 range is a immutable sequence (matlab agar "range" me humne koi value daal di , toh we can't update or change it later on like r = (1,3,4,6) isme hum kuch change or update nahi kar sakte hai , once declared like how we do in variable , ki after declaration we update later in code, like x = 5 and then  x += 1 . We cannot do this with range )
📀 range only contain  "int"  type values.
📀 Every range contain sequence of integers with a common difference(like all ranges are like arithmetic progression. For example:(2,4,6,8,10) , if we say (2,4,5,8,10) this is not a range as their is no common difference )

🟡 How to create a range object or how to declare a range ?
  📀 Like this : [](/Images/39.png)
  📀 Matlab ek range ko hum ese declare karte hai.           r = range(begin , end , common-difference)
                                                          -> Yaha end exclusive hota hai yaani not included.
                                                          -> r = range(2,10,2) then we get in r = (2,4,6,8)
                                                          -> as 10 is not included .
  🟩 Very Important
     [How range works internally through a example ?](/Images/40.png) and [](/Images/41.png)
     
     Toh yeh work ese karta hai ki when we write r = range(2,10,2) , Toh memory me 2 se lekar 9 tak saare number store nahi hote hai balki ek object store hota hai which contain three keys start(begin),stop(end),step(common-difference). Uske baad when we use r in a "for" loop like

     for i in r: 
         print(i)

     and execute this loop then kya hota hai ki sabse pehle ek function run hota hai iter(r) isme parameter me wahi "r" jaata hai which creates a object which we called as "iterator" which stores and tracks the current position yaani current position 0 hai 1 hai 2 hai kya hai, and then next(iterator) karke ek function hota hai jo ki parameter me wahi "iterator" leta hai and uske basis par ek formula which is  
     a+(current position [here,position starts from 0])d where "a" begin element and "d" is common-difference and then jo value aati hai calculate karke , uska check hota hai ki  value < stop hai and if yes then loop me  i = value  ho jaati hai yaani i ki 1st value hume mil jaati hai and then uske baad wo value hum print karte hai and then uske baad kya hota hai ki again current position update hoti hai iterator me and iterator me change hone par next(iterator) chal padta hai and then again same check and we get 2nd value of i and then print and so on till , check false naa ho jaaye , jaise hi check false hota hai control exits out of that loop and this is how range works works internally with loops . 

  📀 Other ways to create range objects :
    1. range(end)                                 here by default begin = 0 hota hai and step = 1
    2. range(begin,end)                           here by default step = 1 hota hai

    -> Matlab hum range ko ese bhi direct likh sakte hai ki :
       range(5) toh iska matlab range(0,5,1) 
                   or 
       range(2,6) iska matlab range(2,6,1)

    -> Example : [](/Images/42.png)