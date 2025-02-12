# The Missing CFO and the Mismatched Fund Valuations

Your company’s **Chief Financial Officer (CFO)** has mysteriously disappeared just days before the annual investment fund performance review! The last anyone heard, they were investigating **discrepancies in fund valuations** across different sources—your company’s internal system and the official custodian bank records.

Concerned about the potential financial impact, the **Operations team** has asked for your help in reconciling the numbers. They believe the CFO was onto something important, and by uncovering the valuation discrepancies, you might find clues about their last steps.

The challenge? The two lists—one from your internal portfolio management system and another from the custodian bank—should **match perfectly**, but they don’t. Your task is to measure how far apart they are.

### **How to reconcile the fund valuations**

Each list contains **Net Asset Values (NAVs)** of multiple investment funds, but they are not ordered the same way. To ensure a fair comparison:

1. **Sort both lists in ascending order.**
2. **Pair each NAV from the internal system with the corresponding NAV from the custodian’s records (smallest with smallest, second smallest with second smallest, etc.).**
3. **Calculate the absolute difference between each pair.**
4. **Sum up all the differences.**

For example, given the following NAV records:

```tsx
Internal System   Custodian Bank
3.00              4.00
4.00              3.00
2.00              5.00
1.00              3.00
3.00              9.00
3.00              3.00
```

Sorting both lists:

```tsx
Internal System:  [1.00, 2.00, 3.00, 3.00, 3.00, 4.00]
Custodian Bank:   [3.00, 3.00, 3.00, 4.00, 5.00, 9.00]
```

Pairing them and calculating the discrepancies:

- **1.00 vs 3.00** → Difference = **2.00**
- **2.00 vs 3.00** → Difference = **1.00**
- **3.00 vs 3.00** → Difference = **0.00**
- **3.00 vs 4.00** → Difference = **1.00**
- **3.00 vs 5.00** → Difference = **2.00**
- **4.00 vs 9.00** → Difference = **5.00**

Total discrepancy: **2.00 + 1.00 + 0.00 + 1.00 + 2.00 + 5.00 = 11.00**

Your actual fund valuation lists contain **many more entries**, and this discrepancy could point to **significant financial risk**. Can you determine the total discrepancy? Solving this might **uncover the CFO’s last steps** and ensure the investment funds remain compliant before the big review! 🚀
