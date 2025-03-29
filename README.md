# Django-Signals
AccuKnox Django Assessment

**Question 1:** By default are django signals executed synchronously or asynchronously? Please support your answer with a code snippet that conclusively proves your stance. The code does not need to be elegant and production ready, we just need to understand your logic.

**Solution: By default, Django signals are executed synchronously. This means they run immediately when the signal is triggered and do not run in a separate thread or process.**

**Question 2**: Do django signals run in the same thread as the caller? Please support your answer with a code snippet that conclusively proves your stance. The code does not need to be elegant and production ready, we just need to understand your logic.

**Solution: Yes, Django signals run in the same thread as the caller. When a signal is emitted, it executes in the same thread that triggered the signal.**

**Question 3:** By default do django signals run in the same database transaction as the caller? Please support your answer with a code snippet that conclusively proves your stance. The code does not need to be elegant and production ready, we just need to understand your logic.

**Solution : Yes, by default, Django signals run in the same database transaction as the caller. However, if an exception occurs in the caller's transaction, any database changes made in the signal will also be rolled back.****
