# 1001: Balance summary

The balance summary displays the balance of each account affected by the transfer log.

Transfer amounts are subtracted from credit accounts and added to debit accounts.

## Acceptance Criteria

* [ ] An error is printed if the prefix or suffix is not consistent between every transfer
* [ ] This case is implemented:

### Log input

| credit    | debit     | balance    |
| --------- | --------- | ---------- |
| liability | expense   | $ 1,000.00 |
| income    | assets    | $ 1,000.00 |
| assets    | liability | $ 1,000.00 |
| income    | assets    | $ 1,000.00 |
| income    | assets    | $ 1,000.00 |
| assets    | equity    | $ 1,000.00 |
| liability | expense   | $ 1,000.00 |

### Balance summary output

| account   | balance        |
| --------- | -------------- |
| income    | ( $ 3,000.00 ) |
| expense   | $ 2,000.00     |
| assets    | $ 1,000.00     |
| liability | ( $ 1,000.00 ) |
| equity    | $ 1,000.00     |