# GetBankAccountResponse

Bank account record matching the provided ID

## Example Usage

```typescript
import { GetBankAccountResponse } from "@maesn/typescript-sdk/models/operations";

let value: GetBankAccountResponse = {
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
  },
  errors: {},
  rawData: {},
};
```

## Fields

| Field                                                                                    | Type                                                                                     | Required                                                                                 | Description                                                                              |
| ---------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------- |
| `meta`                                                                                   | [operations.GetBankAccountMeta](../../models/operations/get-bank-account-meta.md)        | :heavy_minus_sign:                                                                       | N/A                                                                                      |
| `data`                                                                                   | [models.BankAccountResponseDto](../../models/bank-account-response-dto.md)               | :heavy_check_mark:                                                                       | N/A                                                                                      |
| `errors`                                                                                 | [operations.GetBankAccountErrors](../../models/operations/get-bank-account-errors.md)    | :heavy_check_mark:                                                                       | N/A                                                                                      |
| `rawData`                                                                                | [operations.GetBankAccountRawData](../../models/operations/get-bank-account-raw-data.md) | :heavy_check_mark:                                                                       | N/A                                                                                      |