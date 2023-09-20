#Sep 19,2023
---

##hsenidMobile

|**Employeeid**|**EmployeeName**|**Supervisor id**|
|---          |---              |---              |
|001          |"Ron"            |0                |
|002          |"Will"           |1                |
|003          |"john"           |2                |
|004          |"Sam"            |2                |
|005          |"White"          |3                |
|006          |"Snow"           |3                |

>Qustion:Supervisors that have 2 or more than 2 subordinates 

#Cross Product
>e1 x e2

|**Employeeid**|**EmployeeName**|**Supervisor id**|**Employeeid**|**EmployeeName**|**Supervisor id**|
|---          |---              |---              |---          |---              |---              |
|001          |"Ron"            |0                |001          |"Ron"            |0                |
|002          |"Will"           |1                |001          |"Ron"            |0                |
|003          |"john"           |2                |001          |"Ron"            |0                |
|004          |"Sam"            |2                |001          |"Ron"            |0                |
|005          |"White"          |3                |001          |"Ron"            |0                |
|006          |"Snow"           |3                |001          |"Ron"            |0                |
|001          |"Ron"            |0                |002          |"Will"           |1                |
|002          |"Will"           |1                |002          |"Will"           |1                |
|003          |"john"           |2                |002          |"Will"           |1                |
|004          |"Sam"            |2                |002          |"Will"           |1                |
|005          |"White"          |3                |002          |"Will"           |1                |
|006          |"Snow"           |3                |002          |"Will"           |1                |
|001          |"Ron"            |0                |003          |"john"           |2                |
|002          |"Will"           |1                |003          |"john"           |2                |
|003          |"john"           |2                |003          |"john"           |2                |
|004          |"Sam"            |2                |003          |"john"           |2                |
|005          |"White"          |3                |003          |"john"           |2                |
|006          |"Snow"           |3                |003          |"john"           |2                |
|001          |"Ron"            |0                |004          |"Sam"            |2                |
|002          |"Will"           |1                |004          |"Sam"            |2                |
|003          |"john"           |2                |004          |"Sam"            |2                |
|004          |"Sam"            |2                |004          |"Sam"            |2                |
|005          |"White"          |3                |004          |"Sam"            |2                |
|006          |"Snow"           |3                |004          |"Sam"            |2                |
|001          |"Ron"            |0                |005          |"White"          |3                |
|002          |"Will"           |1                |005          |"White"          |3                |
|003          |"john"           |2                |005          |"White"          |3                |
|004          |"Sam"            |2                |005          |"White"          |3                |
|005          |"White"          |3                |005          |"White"          |3                |
|006          |"Snow"           |3                |005          |"White"          |3                |
|001          |"Ron"            |0                |006          |"Snow"           |3                |
|002          |"Will"           |1                |006          |"Snow"           |3                |
|003          |"john"           |2                |006          |"Snow"           |3                |
|004          |"Sam"            |2                |006          |"Snow"           |3                |
|005          |"White"          |3                |006          |"Snow"           |3                |
|006          |"Snow"           |3                |006          |"Snow"           |3                |

#Filter
>empid = supervisor id

|**Employeeid**|**EmployeeName**|**Supervisor id**|**Employeeid**|**EmployeeName**|**Supervisor id**|
|---          |---              |---              |---          |---              |---              |
|001          |"Ron"            |0                |002          |"Will"           |1                |
|002          |"Will"           |1                |003          |"john"           |2                |
|002          |"Will"           |1                |004          |"Sam"            |2                |
|003          |"john"           |2                |005          |"White"          |3                |
|003          |"john"           |2                |006          |"Snow"           |3                |

#Fillter
>e1.Supervisorid !=0 or e2.Supervisorid !=0

|**Employeeid**|**EmployeeName**|**Supervisor id**|**Employeeid**|**EmployeeName**|**Supervisor id**|
|---          |---              |---              |---          |---              |---              |
|002          |"Will"           |1                |003          |"john"           |2                |
|002          |"Will"           |1                |004          |"Sam"            |2                |
|003          |"john"           |2                |005          |"White"          |3                |
|003          |"john"           |2                |006          |"Snow"           |3                |

#Projection
>(e1.employeeName)

|**EmployeeName**|
|---             |
|"Will"          |
|"John"          |
