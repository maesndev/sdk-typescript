# Balance

## Example Usage

```typescript
import { Balance } from "maesn/models";

let value: Balance = {
  amount: 3334.77,
  debitCreditIndicator: "DEBIT",
};
```

## Fields

| Field                                                                             | Type                                                                              | Required                                                                          | Description                                                                       |
| --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- |
| `amount`                                                                          | *number*                                                                          | :heavy_check_mark:                                                                | N/A                                                                               |
| `debitCreditIndicator`                                                            | [models.BalanceDebitCreditIndicator](../models/balance-debit-credit-indicator.md) | :heavy_check_mark:                                                                | N/A                                                                               |