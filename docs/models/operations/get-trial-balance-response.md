# GetTrialBalanceResponse

## Example Usage

```typescript
import { GetTrialBalanceResponse } from "maesn/models/operations";

let value: GetTrialBalanceResponse = {
  meta: {
    warnings: [
      "<value 1>",
      "<value 2>",
    ],
    pagination: {
      total: 3438.77,
      perPage: 5109.63,
      currentPage: 2626.79,
      totalPages: 3561.84,
    },
  },
  data: [
    {
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
      totalCreditAmount: 2115.48,
      totalDebitAmount: 296.14,
      updatedDate: "<value>",
    },
  ],
  errors: {},
  rawData: {},
};
```

## Fields

| Field                                                                                      | Type                                                                                       | Required                                                                                   | Description                                                                                |
| ------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------ |
| `meta`                                                                                     | [models.MetaResponse](../../models/meta-response.md)                                       | :heavy_check_mark:                                                                         | N/A                                                                                        |
| `data`                                                                                     | [models.TrialBalanceResponseDto](../../models/trial-balance-response-dto.md)[]             | :heavy_check_mark:                                                                         | N/A                                                                                        |
| `errors`                                                                                   | [operations.GetTrialBalanceErrors](../../models/operations/get-trial-balance-errors.md)    | :heavy_check_mark:                                                                         | N/A                                                                                        |
| `rawData`                                                                                  | [operations.GetTrialBalanceRawData](../../models/operations/get-trial-balance-raw-data.md) | :heavy_check_mark:                                                                         | N/A                                                                                        |