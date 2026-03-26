# MonthlyValueBalance

## Example Usage

```typescript
import { MonthlyValueBalance } from "@maesn/typescript-sdk/models";

let value: MonthlyValueBalance = {
  amount: 8774.15,
  debitCreditIndicator: "DEBIT",
};
```

## Fields

| Field                                                                                        | Type                                                                                         | Required                                                                                     | Description                                                                                  |
| -------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------- |
| `amount`                                                                                     | *number*                                                                                     | :heavy_check_mark:                                                                           | N/A                                                                                          |
| `debitCreditIndicator`                                                                       | [models.MonthlyValueDebitCreditIndicator](../models/monthly-value-debit-credit-indicator.md) | :heavy_check_mark:                                                                           | N/A                                                                                          |