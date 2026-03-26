# TrialBalanceResponseDto

## Example Usage

```typescript
import { TrialBalanceResponseDto } from "@maesn/typescript-sdk/models";

let value: TrialBalanceResponseDto = {
  accountCode: "<value>",
  accountName: "<value>",
  accountNumber: "<value>",
  balance: {
    amount: 2115.48,
    debitCreditIndicator: null,
  },
  createdDate: "<value>",
  monthlyValues: [],
  openingBalance: {
    amount: null,
    debitCreditIndicator: "DEBIT",
  },
  totalCreditAmount: 300.8,
  totalDebitAmount: 1297.36,
  updatedDate: "<value>",
};
```

## Fields

| Field                                                                                    | Type                                                                                     | Required                                                                                 | Description                                                                              |
| ---------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------- |
| `accountCode`                                                                            | *string*                                                                                 | :heavy_check_mark:                                                                       | N/A                                                                                      |
| `accountName`                                                                            | *string*                                                                                 | :heavy_check_mark:                                                                       | N/A                                                                                      |
| `accountNumber`                                                                          | *string*                                                                                 | :heavy_check_mark:                                                                       | N/A                                                                                      |
| `balance`                                                                                | [models.TrialBalanceResponseDtoBalance](../models/trial-balance-response-dto-balance.md) | :heavy_check_mark:                                                                       | N/A                                                                                      |
| `createdDate`                                                                            | *string*                                                                                 | :heavy_check_mark:                                                                       | N/A                                                                                      |
| `monthlyValues`                                                                          | [models.MonthlyValue](../models/monthly-value.md)[]                                      | :heavy_check_mark:                                                                       | N/A                                                                                      |
| `openingBalance`                                                                         | [models.OpeningBalance](../models/opening-balance.md)                                    | :heavy_check_mark:                                                                       | N/A                                                                                      |
| `totalCreditAmount`                                                                      | *number*                                                                                 | :heavy_check_mark:                                                                       | N/A                                                                                      |
| `totalDebitAmount`                                                                       | *number*                                                                                 | :heavy_check_mark:                                                                       | N/A                                                                                      |
| `updatedDate`                                                                            | *string*                                                                                 | :heavy_check_mark:                                                                       | N/A                                                                                      |