# TrialBalanceResponseDto

## Example Usage

```typescript
import { TrialBalanceResponseDto } from "maesn/models";

let value: TrialBalanceResponseDto = {
  accountCode: "<value>",
  accountName: "<value>",
  accountNumber: "<value>",
  balance: {
    amount: 6397.3,
    debitCreditIndicator: "DEBIT",
  },
  createdDate: "<value>",
  monthlyValues: [],
  openingBalance: {
    amount: 3501.58,
    debitCreditIndicator: "CREDIT",
  },
  totalCreditAmount: 3058.45,
  totalDebitAmount: 8611.01,
  updatedDate: "<value>",
};
```

## Fields

| Field                                               | Type                                                | Required                                            | Description                                         |
| --------------------------------------------------- | --------------------------------------------------- | --------------------------------------------------- | --------------------------------------------------- |
| `accountCode`                                       | *string*                                            | :heavy_check_mark:                                  | N/A                                                 |
| `accountName`                                       | *string*                                            | :heavy_check_mark:                                  | N/A                                                 |
| `accountNumber`                                     | *string*                                            | :heavy_check_mark:                                  | N/A                                                 |
| `balance`                                           | [models.Balance](../models/balance.md)              | :heavy_check_mark:                                  | N/A                                                 |
| `createdDate`                                       | *string*                                            | :heavy_check_mark:                                  | N/A                                                 |
| `monthlyValues`                                     | [models.MonthlyValue](../models/monthly-value.md)[] | :heavy_check_mark:                                  | N/A                                                 |
| `openingBalance`                                    | [models.Balance](../models/balance.md)              | :heavy_check_mark:                                  | N/A                                                 |
| `totalCreditAmount`                                 | *number*                                            | :heavy_check_mark:                                  | N/A                                                 |
| `totalDebitAmount`                                  | *number*                                            | :heavy_check_mark:                                  | N/A                                                 |
| `updatedDate`                                       | *string*                                            | :heavy_check_mark:                                  | N/A                                                 |