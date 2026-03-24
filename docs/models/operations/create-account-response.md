# CreateAccountResponse

## Example Usage

```typescript
import { CreateAccountResponse } from "maesn/models/operations";

let value: CreateAccountResponse = {
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
    balance: 9186.9,
    class: "LIABILITY",
    code: "<value>",
    createdDate: "<value>",
    currency: "INR",
    debitCreditIndicator: "DEBIT",
    description: "gee flawed huzzah appropriate roundabout lazy",
    name: "<value>",
    number: "<value>",
    parentAccountId: "<id>",
    status: "ARCHIVED",
    type: "<value>",
    updatedDate: "<value>",
  },
  errors: {},
  rawData: {},
};
```

## Fields

| Field                                                                                 | Type                                                                                  | Required                                                                              | Description                                                                           |
| ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- |
| `meta`                                                                                | [models.MetaResponse](../../models/meta-response.md)                                  | :heavy_check_mark:                                                                    | N/A                                                                                   |
| `data`                                                                                | [models.AccountResponseDto](../../models/account-response-dto.md)                     | :heavy_check_mark:                                                                    | N/A                                                                                   |
| `errors`                                                                              | [operations.CreateAccountErrors](../../models/operations/create-account-errors.md)    | :heavy_check_mark:                                                                    | N/A                                                                                   |
| `rawData`                                                                             | [operations.CreateAccountRawData](../../models/operations/create-account-raw-data.md) | :heavy_check_mark:                                                                    | N/A                                                                                   |