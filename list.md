🟦 list
📀 list is a class (yaani list is a machine which produces list objects that look like [1,2,3,4,] this )
   🟩 Important Point 
   If x = 5.5 and someone asks us ki x belongs to which class .
   Iska matlab hota hai wo humse puch raha hai ki x ke andar jo
   object hai, wo kis category yaani class se belong karta hai .
   Toh hum kahenge x belongs to float class . Kyuki x ke andar jo
   object stored hai wo float class se belong karta hai .Yaani float
   class yaani float machine ne us object ko produce kiya hai .

   Concept of class (In a different perspective)
   Example : [](/Images/43.png)

   In total ,python have objects that are stored in a variable . 
   These objects are made by class and class is a machine and 
   different class produce different variety or types of objects .
   
📀 list is an iterable sequence

📀 list is mutable (yaani editable )

📀 list is growable (yaani we can insert elements in list and grow it , not like array in C++ and C which is fixed)

📀 list can store heterogeneous data (yaani array me toh hum sirf ek data type ka hi data daal sakte the like [1,2,4,5,6] all are int type only , but list me hum multiple data-types ka data ek hi list me daal sakte hai like [1,2,"hello",3+4j] yaani int , string , complex number and many more ek hi me )

📀 list elements are indexed (yaani same like array , list me bhi numbering hoti hai which starts from 0 )


In total , list bhi ek class hai jo list objects produce karti hai , yeh array ki tarah hi same hoti hai but iski bahut saari properties alag hoti hai like iska size growable hota hai yaani changable and isme hum multiple data types ko ek saath daal sakte hai and many more ... This is called " list " .


🟢 Question :  How a list is saved into the memory ?
   [tHIS IS HOW list memory me store hoti hai ](/Images/55.png) and [](/Images/listmemory.png)


🟨 How to create list objects ?
[We create "list" objects same like we do in arrays ](/Images/44.png)
Example : [](/Images/45.png)

🟨 How to access list elements ?
[We access "list" elements same like we do in arrays ](/Images/47.png)
Example : [](/Images/46.png)

🟨 Concept of Negative Indexing ?
[Yeh concept kehta hai ki "every list object has two indexing" , Pehli toh starts from 0 Left to Right  and dusari hai starts from -1 from Right to Left . Yaani if we have a list l1=[10,20,30,40,50] then               l1[1] = l1[-4] . Iska fayda yeh hota hai ki agar hume last ki side se kisi element ko find karna ho toh hum use easily and instantly find kar sakte hai .](/Images/47.png)

🟨 How to access list elements through "for" and "while" loop ?
[](/Images/49.png) and EXAMPLE : [](/Images/50.png)

🟨 How to delete a element from a list ?
[](/Images/51.png)

🟨 How to edit or update a element of a list ?
🟡 [same like we do in array ](/Images/52.png)
🟢 Agar hum kisi ese element ko update karne ki koshish karte hai jo list me hai hi nahi then we get 
"index" error . [Like yaha we tried to update the value of element which is at index 6 , but index 6 hi nahi hai toh element kaise hoga waha par toh we get the index error , ki aap jis index ko edit krne ki koshish kar rahe hai wo exist hi nahi karta hai, list me](/Images/53.png)

🟨 How to insert any element in a list and how to append (yaani list ke last me daalna) in a list ?
[](/Images/54.png)

🟨 Packing and Unpacking in list ?
[](/Images/56.png)

🟨 Some special Built-in functions for every iterable ?
[](/Images/57.png)

🟨 list() function ?
[It is used for Type-conversion of different iterables to list ](/Images/58.png)

🟨 comparison in list ?
[](/Images/59.png)

🟨 concatenation in list ?
[Hum just like we add two numbers, Similiarly, we can add two lists also .](/Images/60.png)

🟨 repetition in list ?
[](/Images/61.png)

🟨 2D list ?
[](/Images/62.png)

🟨 list object methods ?
[](/Images/63.png) and [](/Images/64.png) and [](/Images/65.png)
🟢 Important Point : sorted() function always list hi return karta hai , no matter what type of iterable we pass in it .
                     Jaisa bhi iterable hum paas karenge , sorted usi iterable ko sort karke uska list return kar dega .
                     Chahe hum str paas kare yaa list yaa dict ya anything , output yaani return is a "list" only .
                     
🟨 list comprehension ?
[](/Images/66.png)