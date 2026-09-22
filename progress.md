## Done

## In progress

## Open / needs a human

### 2026-09-22
- src\main\java\com\example\rewards\service\RewardsService.java:6 — TODO: this calls findAll() once per customer (N+1 pattern); group transactions by customerId in one pass
- src\main\java\com\example\rewards\service\RewardsService.java:9 — TODO: findAll() loads every transaction into memory; add a repository query filtered by customerId
- src\main\java\com\example\rewards\service\RewardsService.java:13 — TODO: add tests for month boundaries (startMonth == endMonth, transaction on the last day of a month)

### 2026-09-22 (re-check)
No new TODOs since 2026-09-22. All 3 known TODOs above still present in code; none removed.
