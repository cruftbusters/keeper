# 1001: filing previews

Filing previews include:

- IRS Form 1120-S (U.S. Income Tax Return for an S Corporation)
- Washington Department of Revenue Business & Occupation Tax

## Acceptance Criteria

- [ ] This case is implemented:

### Input balance summary

| account                                        | balance        |
| ---------------------------------------------- | -------------- |
| income > Gross receipt or sales                | ( $ 3,000.00 ) |
| expense > Compensation of officers             | $ 400.00       |
| expense > Rents                                | $ 400.00       |
| expense > Taxes and licenses                   | $ 400.00       |
| expense > Pension, profit-sharing, etc., plans | $ 400.00       |
| expense > Other deductions > Example deduction | $ 400.00       |
| assets                                         | $ 1,000.00     |
| liability                                      | ( $ 1,000.00 ) |
| equity                                         | $ 1,000.00     |

### Output preview for Form 1120-S

| item                                                             | amount     |
| ---------------------------------------------------------------- | ---------- |
| 1 Gross receipt or sales                                         | $ 3,000.00 |
| 6 Total income (loss)                                            | $ 3,000.00 |
| 7 Compensation of officers                                       | $ 400.00   |
| 11 Rents                                                         | $ 400.00   |
| 12 Taxes and licenses                                            | $ 400.00   |
| 17 Pension, profit-sharing, etc., plans                          | $ 400.00   |
| 20 Other deductions (attach statement)                           | $ 400.00   |
| 21 Total deductions. Add lines 7 through 20                      | $ 2,000.00 |
| 22 Ordinary business income (loss). Subtract line 21 from line 6 | $ 1,000.00 |

| Schedule K > Ordinary business income (loss) (line 22) | $ 1,000.00 |
