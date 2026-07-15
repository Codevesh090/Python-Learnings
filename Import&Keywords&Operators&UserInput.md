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



🟩 Important Point
In python we cannot declare multiple variables like this.       a=5 , b=6 , c=7
          We can only declare it like this ->   a,b,c = 5,6,7



1. Arithmetic Operator

📀 ** (Yeh use hota hai agar hume kisi number ki power nikalni hai)
Example : [](/Images/12.png)


📀 + (Yeh use hota hai agar hume kinhi do number ko add karne ke liye )
Example : [](/Images/13.png)


📀 + (Yeh use hota hai agar hume kinhi do number ko subtract karne ke liye )
Example : [](/Images/14.png)


📀 * (Yeh use hota hai agar hume kinhi do number ko multiply karne ke liye )
Example : [](/Images/15.png)


📀 % (called as Modulus and Yeh use hota hai agar hume kisi number ka remainder nikalna ho )
🟨 Yaha hum if a%b hai and a or b me se koi decimal contained number hai , toh python me uska bhi modulo nikaal sakte hai like            3.5 % 4 = 1.5 (so,here 3.5 is a decimal number used ) 
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


In total |  true division operator accurate mathematical result deta hai but always a float result represented
            floor division operator depends on operands if any of operand is float then answer is in float only



2. Relational Operator (Relational operator ka result hamesha   True or False       hi aata hai)
For example :
                   3 < 4      True
                   5 > 4      False
                   6>5>4      True      (Agar hum yahi operation agar C me karte toh iska answer False aata because In C , calculation ese hota hai ki left to right yaani sabse pehle 6>5 calculate hoga then answer True yaani 1 aayega and then 1>4 calculate hoga and then answer 0 aayega yaani false . That's why in C we get false . But in Python language , left to right hi jaata but calculation ka style alag hota hai , python me pehle 6>5 calculate hoga and if true then 5>4 calculate hoga and if all are true , then the final result comes out to be true . This is How Relational multioperator calculation hoti hai Python me .  )

🟩 If For example like we have a>b>c>f>w then if only all are true then final reult comes out to be "True" and if even one is false then it comes out to be "False" .

and other symbols works same as we know ......



3. Logical Operator (and , or , not)
It is same as we have in C like in C language we have   &&  ,   ||   ,  !
Similiarly, we have here              and , or , not
Example: [](/Images/19.png)  

not - Iska use hota hai statement ke result ko inward yaani ulta karne ke liye 
and - Like if we have (3>0 and 4<1 and 7>3)  then iska matlab if any of statement is false ,whole becomes false
or - Like if we have  (3>0 or 4<1 or 7>3)   then iska matlab if any of statement is true ,whole becomes true

🟩 Important Point
Non-empty string "     "    - considered as "True"
empty string ""             - considered as "False"
Every non-zero number       - considered as "True"
Zero number                 - considered as "False"

🟩 2nd Important Point (Special cases when or , and used with string )
Yaani if some ask ki  "Seeta" or "Geeta"   ka kya result hoga
     Toh answer hai "Seeta" naa ki true or false because this rule is followed 

    Rule 1:
    A or B
    * Agar A truthy hai → A return karo
    * Warna → B return karo. 

    or we can say 
    
    📀 ki jispar result depend hoga wahi result hoga like agar "seeta" hi false ho jaayega jo geeta tak jaana hi nahi padega . Hence , Here result depends on "Seeta" , So, answer is Seeta . 
    

And if someone asks ki  "Seeta" and "Geeta"   ka kya result hoga
     Toh answer hai "Geeta" as now result depends on "Geeta" kyuki 
    
    Rule 2:
    A and B
    * Agar A truthy hai → B return karo
    * Warna → A return karo

    or we can say 

    📀 ki jispar result depend hoga wahi result hoga like here ki agar 1st "Seeta" true bhi ho jaayega toh bhi hum yeh nahi keh sakte hai ki iska result true aayega kyuki agar 2nd bhi true hoga then only we can say the answer is true . So, yaha result depend kar raha hai 2nd par . Hence, final result here is  "Geeta" here . 


Simliary , more examples:
 5 or 0     answer is    5
 5 and 0    answer is    0



4. Bitwise operator
It is used for binary calculation , so leaving it for now.



5. Assignment Operator
Is operator ka use hota hai kisi variable me kuch assign karne ke liye .
It is same like as we know .



6. Identity Operator (is , is not)
🟨 Toh Python me kya hota hai ki agar humne ek code script likhi hai jisme ek variable define kiya hai x = 5 and dusara variable define kiya y = 5 toh python bahut intelligent language hai wo kya karti hai ki do alag-alag object which contain 5 heap space me nahi banayegi . Yaani python kabhi bhi same data ke liye alag-alag memory allocate nahi karti hai heap space me , balki wo kya karti hai ki wo ek hi 5 heap space me banayegi and usko x and y dono se link kar degi yaani jod degi , yaani 5 ki id (address) x me bhi chala jaayega and y me bhi chala jaayega . For example:  [](/Images/20.png) and [](/Images/21.png)

🟨 Toh identity operator kya karta hai , ki wo check karne ka kaam karta hai ki kya koi do refrence variables ke beech same address share hua hai , yaani kya koi do refrence variable same object ko refer kar rahe hai heap space me . For example : [](/Images/22.png)

🟨 And "is not" kya karta hai "is" ka inward result yaani ulta result deta hai , yaani if x and y have same address toh True aana chahiye toh "is not" True ka ulta "False" aayega result.

🟩 In simple terms , "is" checks where x and y have same id and if yes then true else false .
                     "is not" gives the inward decision of "is" .



7. Membership Operator (in , not in)
🟩 Yeh operator kya batata hai ki kya  y me x present hai ?
🟨 But isme ek condition hoti hai ki y should be iterable yaani bada hona chahiye , means yaa toh tuple ho , list ho , range ho , str ho etc.. yaani koi esa data type jo ki collection of elements se bana ho .

🟨 For example : [](/Images/23.png) . Jaise "H" tha "Hello" me toh True and jab nahi tha toh False

🟨 "not in" is a inward of "in" hota hai .Yaani, ulta jaise "H" tha "Hello" me toh False and jab nahi tha toh True


🟥 Left do after 1:06:00 --------------------------------------------------------------------------------------