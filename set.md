🟦 set                               SEE HERE : [](/Images/91.png)
set is a class
set is mutable
set is not a sequence (Matlab "set does not guarantee to store values in order of insertion" . Yaani agar hum set me values daalte hai ek-ek karke like pehle 4 then 5 then 6 then 7 . Toh jaruri nahi hai ki set me value ek sequence me hui ho 4,5,6,7 . set me values kisi bhi order me arranged yaa insert ho sakti hai like 5,6,4,7 or 6,5,7,4 any order. Jabki tumne is order me daala tha 4,5,6,7)
set is iterable (🟢 but "set me indexing nahi hoti hai" , isme hum kisi dusare tareeke se iterate karte hai and also because there is no concept of indexing , toh "slicing operator does not work here" . Kyuki Slicing operator ko kaam karne ke liye index chahiye hote hai , ab index hi nahi hai toh wo kaam kaise karega ).
set cannot contain duplicate values ever .
set can store heterogeneous elements .


🟨 How to declare and initialise set object ?
[This is how we initialise and declare a set](/Images/92.png)
[Some Important Points](/Images/93.png)

🟨 HOW TO ACCESS ELEMENTS of a set ?
[There is only one way to access set elements which is only through a "for-loop" . It is because it does not have concept of indexing. And indexing ka concept bhi isiliye nhi hai kyuki set is not a sequence toh elements kisi bhi order me memory me save ho sakte hai , toh index agar hota bhi hai , toh hume kaise pata chalega ki set[2] karne par konsi value aayegi as we don't know the order.Toh index rakhne ka koi matlab nahi hai . Indexing nahi rakhne ka kaaran , set is not a sequence hi hai ] [Can only be accessed through for-loop](/Images/94.png) and [](/Images/95.png)

🟨 Built-In methods ?
[We have 5 built in methods  len()  , min() , max() , sum() , sorted()  ](/Images/96.png)

🟨 Concatenation , Repetition and Comparison Operator ?
[set does not support concatenation of two sets and also do not support Repetition Operator on a set](/Images/97.png)
[ set me bhi comparison operator same hi kaam karta hai like in other iterables. 
     BUT THER IS A DIFFERENCE WHICH IS :
  -> KI AUR SABHI ITERABLES ME EQUAL HONE KE LIYE , ELEMENTS AND ORDER OF ELEMENTS DONO SAME HONE CHAHIYE BUT IN SET    -> "Two set objects are equal if there elements are same , doesn't matter the order of elements "
](/Images/98.png)

🟨 set objects method ?
-> [Concept of add() , update()](/Images/99.png) and also [Difference between add() and update()](/Images/100.png) 
-> [Concept of remove() , discard() , pop() , clear()](/Images/102.png)
-> [Concept of union() , intersection() , ()issubset , issuperset()](/Images/103.png)

🟨 set comprehension ?
[](/Images/101.png)

-------------------------------------------------------/----------------------------------------------------------------