# GetBankAccountResponse

## Example Usage

```typescript
import { GetBankAccountResponse } from "maesn/models/operations";

let value: GetBankAccountResponse = {
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
  data: {
    id: "<id>",
    balance: 5188.62,
    bankName: "<value>",
    bic: "<value>",
    createdDate: "<value>",
    currency: "LKR",
    description: "across unfortunate altruistic exhausted handover inasmuch",
    fileType: "CSV",
    iban: "AZ79YHWT00300307710301909005",
    name: "<value>",
    number: "<value>",
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
| `meta`                                                                                   | [models.MetaResponse](../../models/meta-response.md)                                     | :heavy_check_mark:                                                                       | N/A                                                                                      |
| `data`                                                                                   | [models.BankAccountResponseDto](../../models/bank-account-response-dto.md)               | :heavy_check_mark:                                                                       | N/A                                                                                      |
| `errors`                                                                                 | [operations.GetBankAccountErrors](../../models/operations/get-bank-account-errors.md)    | :heavy_check_mark:                                                                       | N/A                                                                                      |
| `rawData`                                                                                | [operations.GetBankAccountRawData](../../models/operations/get-bank-account-raw-data.md) | :heavy_check_mark:                                                                       | N/A                                                                                      |