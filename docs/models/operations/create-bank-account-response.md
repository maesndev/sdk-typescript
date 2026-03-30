# CreateBankAccountResponse

Bank account created successfully

## Example Usage

```typescript
import { CreateBankAccountResponse } from "@maesn/typescript-sdk/models/operations";

let value: CreateBankAccountResponse = {
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

| Field                                                                                          | Type                                                                                           | Required                                                                                       | Description                                                                                    |
| ---------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------- |
| `meta`                                                                                         | [operations.CreateBankAccountMeta](../../models/operations/create-bank-account-meta.md)        | :heavy_minus_sign:                                                                             | N/A                                                                                            |
| `data`                                                                                         | [models.BankAccountResponseDto](../../models/bank-account-response-dto.md)                     | :heavy_check_mark:                                                                             | N/A                                                                                            |
| `errors`                                                                                       | [operations.CreateBankAccountErrors](../../models/operations/create-bank-account-errors.md)    | :heavy_check_mark:                                                                             | N/A                                                                                            |
| `rawData`                                                                                      | [operations.CreateBankAccountRawData](../../models/operations/create-bank-account-raw-data.md) | :heavy_check_mark:                                                                             | N/A                                                                                            |