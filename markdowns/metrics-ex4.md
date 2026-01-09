Issue 1: Generic exceptions should not be caught
File: BankAccount.java 160
Explanation: He don't want the code to use a generic `catch (EXception e)` but he wants us to use each specific catch for each errors.

Issue 2: Resources should be closed
File: BankAccount.java 137-140
Explanation: We opened resources that never be closed between each calls.

Issue 3: Cognitive Complexity of methods should not be too high
File: BankAccountApp.java 31
Explanation: The method main it too long and handles too much responsability.

Fix issue 1:
```
// Before
catch (Exception e) { 
    System.out.println("Error reading file"); 
}

// After
catch (java.io.FileNotFoundException e)
{
    ...
}
catch (java.util.NoSuchElementException e)
{
    ...
}
```

Fix issue 2:
```
try (FileInputStream fis = new FileInputStream(text);
     Scanner fileScanner = new Scanner(fis)) {
    while (fileScanner.hasNextLine()) {
        ...
    }
} catch (IOException e) {
    ...
}
```

---

There's a real correlation between huge WMC/CBO classes and the one sonar is mentioning. This proved me that those metrics can help to identify classes that can cause problem in the future.

