🟦 How to define and call a function in python IN-GENERAL ?
[](/Images/116.png) and [](/Images/117.png)

🟦 Types of defining a function ?
[](/Images/118.png) and [](/Images/119.png) and [](/Images/120.png) and [](/Images/121.png) and [](/Images/122.png)
Hamesha pehle dhek lo ki hume kis type ka function banana hai and then uske hissab se function ka structure banao .

🟦 How does code executes in python ?
Python me koi compiler ka concept nahi hota hai like C language . Isme hum apne source code ko compile nahi karte hai .
Toh isme kya hota hai . Python me hota hai "Python interpreter" that's why we say it as a interpreted language .Python Interpreter ek program hota which consists of two parts : Compiler part and PVM part . Compiler part jo kya karta hai ki wo hamare python me likhe hue source code ko leta hai and us code ko yeh line by line phir compile karta hai "Bytecode" me (Bytecode ek intermediate, low-level instruction set hai — machine code yaani binary code nahi hota hai . It is like pieces of instruction like LOAD_CONST, BINARY_ADD, STORE_NAME etc...)and then aata hai dusara program which is Python Virtual Machine(it is also a program , written and compiled in C language called as CPython) . PVM un compiled Bytecodes ko leta hai like BINARY_ADD , STORE_ADD etc.. and then PVM ke andar, har bytecode instruction ke liye pehle se ek C language me function likha hua and compiled form me hota hai .Toh PVM kya karta hai ki wo BYTECODE ko dhek-kar uske corresponding compiled function ko call kar deta hai and then wo function execute hota hai CPU ke through and that's how Python ka koi code execute hota hai . 

Yaani simply :     Python source code -> Converts to Bytecode through Compiler part -> Now,CPU do not understand BYTECODES  -> So, we use PVM -> PVM is program written and compiled in C language -> PVM see the Bytecode and on the basis of that Bytecode it calls its respective function in its compiled Machine code -> Now, that function executes in CPU as that function is compiled means it is in BINARY FORM which CPU understands . Hence, this way Python me code execute hota hai . [SEE HERE VISUALLY](/Images/125.png)

🟨 IMPORTANT POINTS :
❇️ Python me there is no separate compilation step , you just run source code like script.py and it handles translation  and execution together, at runtime. (Yaani like humne ek python code likha , toh esa nahi hoga like C language pehle compile karenge and then run karenge , Isme hum direct run karte hai and then python interpreter use compile bhi karega and execute bhi at runtime . Isiliye hum kehte hai ki Python hai "Just-In Time compilation language" and C language have "Ahead of time compilation language" )

❇️ To run a python code we need to have python interpreter yaani Compiler part + PVM part . Then only python executes .
   Toh jab hum Python install karte hai python.org se toh us time par , hamari machine me dono hi part install ho jaata hai baaki package ke saath .
   
❇️ [Difference between C language and Python language in code execution process](/Images/124.png)

❇️ [Browser se jab hum koi app download karte hai jo python me likhi gayi hai , wo kaise chalti hai . Kyuki hum toh direct app download kar rahe hai , hamare paas toh python interpreter installed hi nahi hai ? ](/Images/126.png)

❇️ Python me bhi compile time par "error" aata hai if it hits any Syntax Error, ese python me koi compile time nahi hota hai but when we run a python source code then through python interpreter , compile part yaa interpretation time jisme bytecode me conversion hota hai , us time par error aa jaata hai if it encounters any syntax error in our python code .


🟦 How does variables and function executes in python ?
[](/Images/133.png)  and  [](/Images/134.png)   and   [](/Images/135.png)   and    [](/Images/136.png)
and the ultimate resource is "In folder "excalidrawcpp" SEE -> Python-function-variable-execution.excalidraw"
----------------------------------------------------------------/-------------------------------------------------------
🟦 Types of parameters 
1. Default Parameters
   [What is a default parameter](/Images/127.png) and [Rule of default parameter to follow](/Images/128.png)
2. Positional Parameters
   [What is a positional parameter](/Images/129.png) 
3. Keyword Parameters
   [What is a keyword parameter](/Images/130.png) 
4. Mixed Parameters
   [How to use Mixed parameters: Rule 1](/Images/131.png) and [How to use Mixed parameters: Rule 2](/Images/132.png)
----------------------------------------------------------------/-------------------------------------------------------