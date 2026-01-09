Proof that is working:
```
[INFO] 
[INFO] Results:
[INFO] 
[INFO] Tests run: 62, Failures: 0, Errors: 0, Skipped: 0
[INFO] 
[INFO] 
[INFO] --- jar:3.3.0:jar (default-jar) @ bank ---
[INFO] ------------------------------------------------------------------------
[INFO] BUILD SUCCESS
[INFO] ------------------------------------------------------------------------
[INFO] Total time:  1.092 s
[INFO] Finished at: 2026-01-09T11:33:25+01:00
[INFO] ------------------------------------------------------------------------
```

---

So maven clean:
Will only execute phase `clean` which will delete all content from `target`

Test:
Will run `validate` -> `compile` -> `test-compile` -> `test`, but will fill `target`

Package:
Will run all the phase to `package` ands it will fill `target` with jar and other usefull file for maven.