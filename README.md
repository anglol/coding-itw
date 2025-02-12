# The Missing CFO and the Mismatched Fund Valuations

It’s year-end, and everything is running smoothly—except for one thing. Your CFO is on a well-deserved surprise getaway to the Bahamas, leaving the finance team to finalize the fund valuations before the reporting deadline! 🌴🏖️

Two key reports—the internal ledger and the third-party audit—need to be aligned before they are finalized. Both lists contain fund valuations based on unique identifiers, but when the team compares them side by side, they notice some small differences. Since different sources can sometimes round or calculate values slightly differently, your job is to measure the total variation between the two lists and ensure everything is on track.

To do this, you’ll match the smallest number in the internal report with the smallest in the audit report, the second-smallest with the second-smallest, and so on. Then, sum up the absolute differences between each pair to measure the total variance.

For example, if the two reports contain:

```tsx
Internal System   Audit Report
3.00              4.00
4.00              3.00
2.00              5.00
1.00              3.00
3.00              9.00
3.00              3.00
```

Sorting and pairing the values:

- 1 (internal) vs 3 (audit) → difference = 2
- 2 vs 3 → difference = 1
- 3 vs 3 → difference = 0
- 3 vs 4 → difference = 1
- 3 vs 5 → difference = 2
- 4 vs 9 → difference = 5

Total variance: 2 + 1 + 0 + 1 + 2 + 5 = 11

Your [actual reports](https://github.com/anglol/coding-itw/blob/main/dataset.txt) contain many more fund valuations. Can you determine the total variance and help the team wrap up the reconciliation process?
