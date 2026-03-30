# GetTrialBalanceResponse

Trial balance for the authenticated end user's connected target system

## Example Usage

```typescript
import { GetTrialBalanceResponse } from "@maesn/typescript-sdk/models/operations";

let value: GetTrialBalanceResponse = {
  data: [
    {
      accountCode: "<value>",
      accountName: "<value>",
      accountNumber: null,
      balance: {
        amount: 2115.48,
        debitCreditIndicator: null,
      },
      createdDate: "<value>",
      monthlyValues: [
        {
          month: null,
          balance: {
            amount: 6542,
            debitCreditIndicator: null,
          },
        },
      ],
      openingBalance: {
        amount: null,
        debitCreditIndicator: "DEBIT",
      },
      totalCreditAmount: 7668.05,
      totalDebitAmount: 6052.39,
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
| `meta`                                                                                     | [operations.GetTrialBalanceMeta](../../models/operations/get-trial-balance-meta.md)        | :heavy_minus_sign:                                                                         | N/A                                                                                        |
| `data`                                                                                     | [models.TrialBalanceResponseDto](../../models/trial-balance-response-dto.md)[]             | :heavy_check_mark:                                                                         | N/A                                                                                        |
| `errors`                                                                                   | [operations.GetTrialBalanceErrors](../../models/operations/get-trial-balance-errors.md)    | :heavy_check_mark:                                                                         | N/A                                                                                        |
| `rawData`                                                                                  | [operations.GetTrialBalanceRawData](../../models/operations/get-trial-balance-raw-data.md) | :heavy_check_mark:                                                                         | N/A                                                                                        |