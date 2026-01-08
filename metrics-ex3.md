Classe          | LOC   | WMC   | CBO   | LCOM  | Quick notes
Person          | ~235  | 31    | 1     | Low   |
Bank            | ~175  | 38    | 7     | Moyen |  
BankAccount     | ~180  | 35    | 5     | Élevé |
BankAccountApp  | ~220  | 28    | 5     | N/A   |

Highest WMC is Bank and highest CBO is Bank.

I'm worrying about the main class in BankAccountApp because it's one single huge fonction. Which if this needs maintenance it will very hard to modify something inside.