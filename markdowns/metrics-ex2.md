1 :

Class           | LOC   | WMC   | CBO   | LCOM 
BankAccount	    | 462   | 20    | 6     | 44

2:
Choosed method public boolean `withdrawMoney(double withdrawAmount)`

3:
cyclomatic complexity value = 5
Since we have 1 base + 4 sub conditions

4:
My propostion to refractor this function would be create another function named `canWidthdraw(double amount)`.
So we can move the huge if condition `withdrawAmount >= 0 && balance >= withdrawAmount && withdrawAmount < withdrawLimit && withdrawAmount + amountWithdrawn <= withdrawLimit` to `canWidthdraw`.
The function will look actually better and we can understand that we check if we can widthdraw.