Class           | LOC   | NOM   | Short description of responsibility
Bank            | 413   | 12    | Create and delete account, get accounts balance metrics
BankAccount     | 462   | 18    | Manage account parameters (balance, authors, etc)
person          | 327   | 21    | Manage a person identity (age, sex, weight, eye color, etc)
BankAccountApp  | 491   | 2     | Use all the other classes to run the app

> Note WMC seems be different from NOM: me personnal explantion is maybe the tool is ignoring constructors and certains functions.

Commands outputs:
```
java -jar ckjm_ext.jar target/classes/bankAccountApp/Bank.class 
bankAccountApp.Bank 14 1 0 3 44 0 0 3 12 0,8333 413 1,0000 0 0,0000 0,3286 0 0 28,0714

java -jar ckjm_ext.jar target/classes/bankAccountApp/BankAccount.class 
bankAccountApp.BankAccount 20 1 0 2 43 44 0 2 18 0,6908 462 1,0000 0 0,0000 0,2917 0 0 21,7000

java -jar ckjm_ext.jar target/classes/bankAccountApp/Person.class 
bankAccountApp.Person 23 1 0 0 40 79 0 0 21 0,7626 327 0,8889 0 0,0000 0,3565 0 0 12,8261

java -jar ckjm_ext.jar target/classes/bankAccountApp/BankAccountApp.class 
bankAccountApp.BankAccountApp 2 1 0 3 36 1 0 3 2 2,0000 491 0,0000 0 0,0000 0,5000 0 0 244,5000
```