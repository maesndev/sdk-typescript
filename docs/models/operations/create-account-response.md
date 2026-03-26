# CreateAccountResponse

## Example Usage

```typescript
import { CreateAccountResponse } from "@maesn/typescript-sdk/models/operations";

let value: CreateAccountResponse = {
  data: {
    id: "<id>",
    balance: 5109.63,
    class: "EQUITY",
    code: "<value>",
    createdDate: "<value>",
    currency: "KES",
    debitCreditIndicator: "CREDIT",
    description: "frantically pfft whereas so limp impressionable within",
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
| `meta`                                                                                | [operations.CreateAccountMeta](../../models/operations/create-account-meta.md)        | :heavy_minus_sign:                                                                    | N/A                                                                                   |
| `data`                                                                                | [models.AccountResponseDto](../../models/account-response-dto.md)                     | :heavy_check_mark:                                                                    | N/A                                                                                   |
| `errors`                                                                              | [operations.CreateAccountErrors](../../models/operations/create-account-errors.md)    | :heavy_check_mark:                                                                    | N/A                                                                                   |
| `rawData`                                                                             | [operations.CreateAccountRawData](../../models/operations/create-account-raw-data.md) | :heavy_check_mark:                                                                    | N/A                                                                                   |