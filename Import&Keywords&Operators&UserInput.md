🟦 import
Toh import keyword samajhne ke liye we have to firstly understand "module" kya hota hai .

🟡 module

📀 Agar python me hum koi file banaye and usme kuch python code likhe and save it with file extension   .py
📀 Then us file ko hum ek module kehte hai . Yaani normaly a "python file" is called as a "module" .

📀 Every python module contains me 3 types ke reusable elements .
   1. variables (In python , variable refers to that refrence variable that refers a instance object)
   2. functions (In python , function refers to that refrence variable that refers a function object)
   3. classes   (In python , class refers to that refrence variable that refers a class object)
Yaani har python file me every variable,function and classes are reusable and can be used in other files also.

📀 Toh agar hum kisi python module ke reusable elements ko use karna chahte hai , yaani un refrence variables ka use karna chahte hai kisi dusari file me , So we follow two steps are : 
1. Do         ->         import filename
2. Use it like   ->                              filename.variablename

📀 Important Point : The location of   "Our python file"    and     "Refrence module"     has to be the same .
                    
                    Like :            "My.py"  and  "Ref.py"      has to be under same      "folder"


📀 Example:
[You can see here , how we imported and printed value of x from Ref.py to My.py with under same folder location](/Images/9.png)



🟦 Keywords
🟡 Python me keywords kuch predefined or special reserved words hote hai jinka meaning compiler yaa interpreter ko pehle se hi pata hota hai .

🟡 Remember : print() yaa len() yaa type() etc.. predefined function are not keywords yaani predefined functions alag hote hai and keywords alag hote hai .

🟡 How to use Keywords ?
We can use it directly anywhere as it is a inbuilt into Python's grammer .
When Python reads your program, it first parses the code and immediately recognizes it as a language keyword.

🟡 JUST FOR FUN ---
Toh jab hum browser se python download karte hai jo usi me ek built-in python module download hota hai jiska naam hota hai keyword.py jisme ek list(yaani python me array nahi list hoti hai) hoti jiska naam hota hai "kwlist" . It is a instance object . Toh isi kwlist me sabhi keywords likhe hote hai . So,if we want to print and see all the keywords present in that kwlist then we do the same as we import and use the module .

1. Do                                                                     import keyword
2. Then access its content or keywords like                               print(keyword.kwlist)

Example : [Wrote the python code and run it and got all the keywords](/Images/10.png)

🟩 Important Point
We have three special keywords in our kwlist :
True
False
None (None here in python is same like Null in Javascipt)
because they act as a assignable data to a variable , Yaani hum in keywords ko as a data bhi use kar sakte hai.
and variables me assign bhi kar sakte hai is data ko like    x = True  or   x = False  or   x = None 


🟦 Operators
We have 7 types of operators : [](/Images/11.png)

1. Arthmetic Operator            ** , / , // , * , % , + , -
2. Relational Operator                                                         > , < , >= , <= , == , !=
3. Logical Operator            not , and , or
4. Bitwise Operator                                  & , | , ^ , ~ , >> , <<
5. Assignment Operator          = , += , -= , /= , //= , %= , **= , *= , &= , |= , ^= , ~= , >>= , <<=     
6. Identity Operator           is    ,   is not  
7. Membership Operator                                 in , not in

🟡 Python me increment ++ and decrement -- operator nahi hota hai .





1. Arthmetic Operator

📀 ** (Yeh use hota hai agar hume kisi number ki power nikalni hai)
Example : [](/Images/12.png)


📀 + (Yeh use hota hai agar hume kinhi do number ko add karne ke liye )
Example : [](/Images/13.png)


📀 + (Yeh use hota hai agar hume kinhi do number ko subtract karne ke liye )
Example : [](/Images/14.png)


📀 * (Yeh use hota hai agar hume kinhi do number ko multiply karne ke liye )
Example : [](/Images/15.png)


📀 % (called as Modulus and Yeh use hota hai agar hume kisi number ka remainder nikalna ho )
Example : [](/Images/16.png)


📀 / (called a true division operator )
🟨 Yeh operator ka use hum do number ko divide karne ke liye karte hai but this is a special operator kyuki when we do divide using this operator . Toh hume wahi answer milta hai jo actual mathematically aana chahiye do numbers ko divide karke .
🟨 Matlab agar hum python me.        3/4 kare toh hume answer aata hai 0.75 jo ki mathematically accurate hai.
🟨 But agar yahi kaam hum C me karte toh waha       3/4 karne par answer 0 aata tha , 
🟨 Kyuki waha answer depend karta tha operands par yaani un numbers par jo use ho rahe hai , yaani like 3 is a int and 4 is a int .Toh answer jo aayega wo bhi int hona chahiye isiliye answer 0 aa jata hai .Yaani other languages me answer operators ke data type par depend karta tha .
🟨 This is the difference in using this operator in python and in other languages .
🟩 Also, true division operator always give the answer  as   "float" 
Example : [](/Images/17.png)


📀 / (called a floor division operator )
🟨 Yeh operator bhi division ke liye hi use hota hai but yeh behave karta hai us division operator ki tarah jo C language me use hota hai yaani iska answer depends on this operands data type .
🟩 Yaani if write  ->      a/b  then if a or b is a float then answer always comes as a float .
                           but if both are int only then answer comes as a int only .
Example : [](/Images/18.png)






2. Relational Operator