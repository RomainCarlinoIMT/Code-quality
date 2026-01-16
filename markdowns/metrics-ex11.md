CucumberTests passes:
```
[INFO] -------------------------------------------------------
[INFO]  T E S T S
[INFO] -------------------------------------------------------
[INFO] Running bankAccountApp.AllTests
[INFO] Tests run: 33, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 0.486 s -- in bankAccountApp.AllTests
[INFO] Running bankAccountApp.RunBankAccountCucumberTest

Scenario: A new account has zero balance # src/test/resources/features/bank_account_basic.feature:2
  Given I have a new bank account        # bankAccountApp.BankAccountBasicSteps.i_have_a_new_bank_account()
  When I check its balance               # bankAccountApp.BankAccountBasicSteps.i_check_its_balance()
  Then the balance should be 0           # bankAccountApp.BankAccountBasicSteps.the_balance_should_be(java.lang.Integer)
[INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 0.242 s -- in bankAccountApp.RunBankAccountCucumberTest
```