# TDD workshop - giugno 2025

### Slides

https://docs.google.com/presentation/d/1ewWFtGaiH3-9mx44YfGG7cbvaaGaknel/edit?usp=sharing&ouid=109663187221444318309&rtpof=true&sd=true

### Final Code

The final code is in the branch `workshop-end`: https://github.com/firenzedev/tdd-workshop/tree/workshop-end

### Rules:

1. Add a small test.
2. Run all the tests and fail.
3. Make a small change.
4. Run tests and succeed.
5. Refactor to remove duplication.

### Introduction

We want to create a multi-currency report, like this:

| **Supplier** | **Quantity** | **Price** | **Total** |
| --- | --- | --- | --- |
| CodeCorp | 1000 | 25 USD | 25000 USD |
| BugBusters | 400 | 150 CHF | 60000 CHF |
|  |  |  |  |
| **Total** |  |  | 65000 USD |

We also need to specify exchange rates:

| **From** | **To** | **Rate** |
| --- | --- | --- |
| CHF | USD | 1.5 |

Thinking about what we want to achieve, I wrote some tasks to guide us during development:

- [ ]  generate report
- [ ]  1000 x 25USD + 400 x 150CHF = 65000USD when the rate is 2:1
- [ ]  `$5 + 10 CHF = $10` if rate is 2:1
- [ ]  `$5 * 2 = $10`
- [ ]  [ ]
