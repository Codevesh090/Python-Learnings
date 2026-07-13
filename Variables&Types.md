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
📀 For example : [](/Images/3.png) 
