# MonthlyValue

## Example Usage

```typescript
import { MonthlyValue } from "maesn/models";

let value: MonthlyValue = {
  month: 5883.46,
  balance: {
    amount: 6397.3,
    debitCreditIndicator: "DEBIT",
  },
};
```

## Fields

| Field                                  | Type                                   | Required                               | Description                            |
| -------------------------------------- | -------------------------------------- | -------------------------------------- | -------------------------------------- |
| `month`                                | *number*                               | :heavy_check_mark:                     | N/A                                    |
| `balance`                              | [models.Balance](../models/balance.md) | :heavy_check_mark:                     | N/A                                    |