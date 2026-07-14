🟦 Comments in Python (Ignored by interpreter or compiler when processing code)
🟡 For Single line Comments we use a hashtag ' # '
🟡 Python does not have a dedicated syntax for multi-line comments .
For Example : [](/Images/1.png)


🟦 Variables in Python
🟡 Python is a dynamically typed language , yaani like C yaa C++ me hum declare karte time define karte the ki variable ka type kya hoga like " int a = 5; " toh use hum bolte the statically typed language kyuki usme hume sab kuch batana pad raha tha , But in Python we do not have to define to declare a variable , Bus yaha hume direct likhna hota hai like " a=5 " and automatically jis type ka data hum us variable me daalte hai wahi us variable ki type ban jaati hai . That's why we call it as dynamically typed language .

🟡 Rules to follow while writing a variable name 
📀 Variable name is a combination of         alphabet  |  digit  |  underscore . 
📀 Variable name      cannot start with a digit .
📀 Variable names are       case sensitive .
📀 Keywords     cannot be used as a variable name .


🟦 Important Point
🟡 Jab tak python me hum variables ke andar kuch daalte nahi hai , tab tak wo variable declare nahi hota hai aur hume <name error milta hai> . name error milne ka matlab hai ki wo variable declare nahi hua hai and hum use use karne ki try kar rahe hai .
📀 Like in this example : [](/Images/2.png)
📀 Humne x = x + 5 likha , toh kyuki pehle toh x+5 process hoga and then x declare hoga . But    x+5 ko process karne ke liye is x + 5 me x toh pehle declare hona chahiye na . Toh x toh humne declare hi nahi kiya tha pehle so, we get the <name error> .In total , python me sirf x likh dene se x declare nahi hoga , x = 5 yaani x me koi value daalne ke baad hi wo declare hoga .
🟡 Python me we can change the value of a variable as well as type of variable also .
Yaani like C me agar hum declare kar dete the " int x = 5 " toh hum baad me sirf us variable ki value change kar sakte yaani update kar sakte the like x = 6 not! its type like int to bool or some other . But in python agar hume declare kar diya x = 5 then we can update both the value and the type of the variable x = 2.8 like from int 5 to float 2.8 | 
📀 For example : [](/Images/3.png)  and  [](/Images/4.png)


🟦 In Python , Data Types are categorized into three parts : [](/Images/5.png)
1. Numbers
2. Boolean
3. String

Numbers:                   Boolean:                                 String 
int (x = 5)                bool (x = True or x = False)             str ( x = "Hello" )

float (x = 5.6)

complex (haa python me complex numbers bhi likh sakte hai, For Example: x = 3 + 4j means complex number format)

🟡 Remember : Integer yaa String yaa Boolean naam ka koi data type nahi hota hai | int,str,bool is a data type.
🟡 Remember : In Python,there is no data type "double" and "char" .



🟦 type()
type() is a predefined function , jisme agar hum kisi variable ko as a parameter daalkar call kare toh we get the data type of that variable in return . For example : [](/Images/6.png)

🟡 Remember : In Python,data type is always a "class" in python . Matlab jaise C , C++ , Java me int , bool etc. data types keyword hote the which we use like int a = 5; but python me yeh data-types keyword nahi , ek "class" hoti hai .



🟦 Automatic Memory Management (Now,will understand ki python me automatic memory management ka kya matlab hai)
🟡 Toh jab hum x = 5 likhte hai . Toh Python me memory is divided in two spaces :  Stack Space | Heap Space
🟡 Toh sabse pehle Heap space me ek memory space yaa memory block define hota hai , us block ko hum kehte hai "object" and us object me value jaati hai 5 and Stack side bhi ek memory block banta hai jiska naam hoga "x"
and abhi tak us block me koi value nahi gayi hai.Uske baad kya hota hai ki Heap space side me object ka koi naam nahi hota hai uska sirf ek id yaa address yaa refrence hota hai . Now, ab wo address jaakar us x me store ho jaata hai and that's how a variable is declared in Python memory . Now, iske baad let say humne next line of code me likha hai x = 7 yaani humne x ki value next line me update kar di hai . Toh memory me hota kya hai , toh hota yeh hai ki phir se again heap side ka ek new object banega yaani new memory block defined and usme 7 store ho jaayega and this object also have a id . Now, ab Stack side wapas se new x nahi banega , balki pehle se bane hue x me jo address hoga wo delete ho jaayega and heap me jaha new object bana new memory block uska address store ho jaayega yaani new refrence created in x and ab heap me jo object humne banaya tha pehle jisme 5 tha , kyuki ab uska koi refrence nahi hai stack side toh wo as a "garbage block" ban jaayega and kyuki python  garbage ko khud hi delete kar deta hai garbage , isiliye we say ki in python me automatic memory management ho jaati hai . But in other languge yeh kaam hume khud hi karana padta hai like in C and C++ . 

🟡 Remember : HAR WO MEMORY BLOCK IN HEAP SPACE , JISKA KOI REFRENCE YAA VARIABLE STACK SIDE PAR NAHI HOTA HAI , WO EK GARBAGE BLOCK KEHLATA HAI 
🟡 Remember : Stack space side sirf pointers(yaani address) hi store hote hai , koi data nahi .


🟦 VERY IMPORTANT POINT
Python and C++ dono me runtime par hi stack and heap banta hai and memory allocation hota hai but
C++ aur C jaisi languages me compile time par hi decide ho jaata hai ki every variable ka type (int, double, Student, etc.) and Uska size (sizeof(int), sizeof(Student)) yaani memory layout pehle hi decide ho jaata hai ki kis variable ke liye runtime par kitni memory allocate hogi . But python me memory layout direct runtime par hi decide hota hai because C++ ko isliye banaya gaya tha ki program bahut fast chale aur programmer ko memory par control mile and Python isliye such that code likhna easy hona chahiye variable ka type mat batao, automatically Python khud hi kar lega run time par ,usse pehle tumhe jo ched-chaad karni hai kar lo .

Runtime yaani .exe file ko run karne se run hone ke beech ka time .
Runtime me hi Stack and Heap banta hai and memory allocate hoti hai and then one by one to CPU and execution
And we see a software running in our PC


🟡 For Example : [BEFORE when x = 5 ](/Images/7.png)
                 [AFTER when x = 7 ](/Images/8.png)           -- For refrence : watch from 45:00      Lecture 2


🟡 Remember : Sirf yeh memory block ko hi hum python me "object" nahi kehte hai balki jo data uske andar jaata hai wo always ek object hi hota hai. Kyuki python me x = 5 likhne par sirf 5 hi store nahi hota hai balki yeh store hota hai jisme yeh sab (Memory + Data + Type Information + Behavior (methods) + kuch internal metadata) included rehta hai ,  {Yaani python me variable me kuch bhi store kare that is a object in memory , isiliye toh python variables ki type "class" aati hai naa ki ek keyword kyuki wo value class me jaati hai , class us value ko leta hai usse ek predefined object shape me convert karta hai and then wo object memory me store hota hai } -------For Example:

x = 5 becomes
+-----------------------+
| Integer Object        |
| value = 5             |
| type = int            |
+-----------------------+

Yeh objects bhi divided hai three types me based on data types :

🟦 Types of objects | that are stored in heap space.
🟡 Instance objects
🟡 Function objects 
🟡 Class objects

🟦 print()
It is a predefined function used to print value of a variable , string or expression same like console.log()

🟥 Left do after 1:00:00 --------------------------------------------------------------------------------------