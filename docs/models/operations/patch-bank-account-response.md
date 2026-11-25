# PatchBankAccountResponse

Bank account updated successfully

## Example Usage

```typescript
import { PatchBankAccountResponse } from "@maesn/typescript-sdk/models/operations";

let value: PatchBankAccountResponse = {
  data: {
    id: "<id>",
    balance: 4752.58,
    bankName: null,
    bic: "<value>",
    createdDate: "<value>",
    currency: "GEL",
    description: null,
    fileType: null,
    iban: "FR906869700894G19162230HT12",
    name: "<value>",
    number: null,
    system: "<value>",
    status: "ACTIVE",
    type: "<value>",
    updatedDate: "<value>",
    version: 7813.99,
  },
  errors: {},
  rawData: {},
};
```

## Fields

| Field                                                                                        | Type                                                                                         | Required                                                                                     | Description                                                                                  |
| -------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------- |
| `meta`                                                                                       | [operations.PatchBankAccountMeta](../../models/operations/patch-bank-account-meta.md)        | :heavy_minus_sign:                                                                           | N/A                                                                                          |
| `data`                                                                                       | [models.BankAccountResponseDto](../../models/bank-account-response-dto.md)                   | :heavy_check_mark:                                                                           | N/A                                                                                          |
| `errors`                                                                                     | [operations.PatchBankAccountErrors](../../models/operations/patch-bank-account-errors.md)    | :heavy_check_mark:                                                                           | N/A                                                                                          |
| `rawData`                                                                                    | [operations.PatchBankAccountRawData](../../models/operations/patch-bank-account-raw-data.md) | :heavy_check_mark:                                                                           | N/A                                                                                          |