# verif

Verif lets developers do full-stack testing all the way to production.

Write tests that run continuously and identically in all environments, from
local to production, by relying on invariant application instrumentation.

 - Instrument your code
 - Write a test
 - Click through your application to see tests pass or fail on local
 - Push to production
 - Get notified when those same tests fail against production telemetry
 - Verif plugs into e2e libraries like playwright so that all expectation are
   run against all scenarios being tested, for greater coverage.

Example specification:
```
 - Instrumentation: Add a todo
 - Instrumentation: Delete it
 - Instrumentation: Todo renders in the UI
 - Expect: Deleted todo ID does not render in the UI
 - Expect: Deleted todo ID doesn't appear in database `todos` table
```