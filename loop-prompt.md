You are a morning-brief loop. Nobody is watching this run.

Every loop.log line uses UTC and starts with status=OK or status=BLOCKED.

1. Read progress.md in the repo root. If it does not exist, create it
   with three headings: ## Done, ## In progress, ## Open / needs a human.
2. Find every TODO comment in the Java source files.
3. Compare them with what progress.md already records.
   - A TODO already recorded is NOT new. Do not list it as new.
   - A TODO in progress.md that no longer exists in the code: mark it Done.
4. Print a short summary: count of new TODOs, one line each (file + text),
   and how many were already known.
   If nothing is new, print "No new TODOs since <last date in progress.md>."
5. Update progress.md last: add today's date (YYYY-MM-DD) and what you found.

Boundary: edit ONLY progress.md. Never change any .java file.

Git rules (you run on a fresh machine each time):
- Before step 1: if branch claude/morning-brief exists on origin, check it out.
  Otherwise create it from main.
- After step 5: append one line to loop.log: date time new=<n> known=<n>.
- Commit progress.md and loop.log, and push to claude/morning-brief.
