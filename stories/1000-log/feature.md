# 1000: log

## Acceptance Criteria

- [ ] When page is filled with these transfer values then there is no error:

### Case: Happy path

| credit    | debit     | amount     |
| --------- | --------- | ---------- |
| liability | expense   | $ 1,000.00 |
| income    | assets    | $ 1,000.00 |
| assets    | liability | $ 1,000.00 |
| income    | assets    | $ 1,000.00 |
| income    | assets    | $ 1,000.00 |
| assets    | equity    | $ 1,000.00 |
| liability | expense   | $ 1,000.00 |

### Case: Negative amount

| credit    | debit   | amount     |
| --------- | ------- | ---------- |
| liability | expense | ( $ 1.00 ) |

### Case: questionable inputs

| credit | debit | amount              |
| ------ | ----- | ------------------- |
| 1      | 0     | could be anything   |
| 1.0    | 0.0   | could be 4nyth 1 ng |

- [ ] Amount is composed of a prefix, sign, significand, characteristic, and suffix
- [ ] Prefix and suffix are text; sign is boolean; significand is a whole number; characteristic is an integer
- [ ] Transfers are persisted between page loads
