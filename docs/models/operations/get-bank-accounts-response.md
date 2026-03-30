# GetBankAccountsResponse

List of bank accounts for the authenticated end user's connected target system

## Example Usage

```typescript
import { GetBankAccountsResponse } from "@maesn/typescript-sdk/models/operations";

let value: GetBankAccountsResponse = {
  data: [],
  errors: null,
  rawData: {},
};
```

## Fields

| Field                                                                                      | Type                                                                                       | Required                                                                                   | Description                                                                                |
| ------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------ |
| `meta`                                                                                     | [operations.GetBankAccountsMeta](../../models/operations/get-bank-accounts-meta.md)        | :heavy_minus_sign:                                                                         | N/A                                                                                        |
| `data`                                                                                     | [models.BankAccountResponseDto](../../models/bank-account-response-dto.md)[]               | :heavy_check_mark:                                                                         | N/A                                                                                        |
| `errors`                                                                                   | [operations.GetBankAccountsErrors](../../models/operations/get-bank-accounts-errors.md)    | :heavy_check_mark:                                                                         | N/A                                                                                        |
| `rawData`                                                                                  | [operations.GetBankAccountsRawData](../../models/operations/get-bank-accounts-raw-data.md) | :heavy_check_mark:                                                                         | N/A                                                                                        |