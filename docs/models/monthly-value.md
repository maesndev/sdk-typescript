# MonthlyValue

## Example Usage

```typescript
import { MonthlyValue } from "@maesn/typescript-sdk/models";

let value: MonthlyValue = {
  month: 1173.56,
  balance: {
    amount: 6542,
    debitCreditIndicator: null,
  },
};
```

## Fields

| Field                                                            | Type                                                             | Required                                                         | Description                                                      |
| ---------------------------------------------------------------- | ---------------------------------------------------------------- | ---------------------------------------------------------------- | ---------------------------------------------------------------- |
| `month`                                                          | *number*                                                         | :heavy_check_mark:                                               | N/A                                                              |
| `balance`                                                        | [models.MonthlyValueBalance](../models/monthly-value-balance.md) | :heavy_check_mark:                                               | N/A                                                              |