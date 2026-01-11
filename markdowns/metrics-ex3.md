Classes         | LOC   | WMC   | CBO   | LCOM 
Person          | 327   | 23    | 0     | 79
Bank            | 413   | 14    | 3     | 0  
BankAccount     | 462   | 20    | 2     | 44
BankAccountApp  | 419   | 2     | 3     | 1 (very suspicous since there's only one method)

Highest WMC is Person and highest CBO is BankAcountApp.

I'm worrying about the main class in BankAccountApp because it's one single huge fonction. Which if this needs maintenance it will very hard to modify something inside.