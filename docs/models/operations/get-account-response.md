# GetAccountResponse

Account record matching the provided ID

## Example Usage

```typescript
import { GetAccountResponse } from "@maesn/typescript-sdk/models/operations";

let value: GetAccountResponse = {
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

| Field                                                                           | Type                                                                            | Required                                                                        | Description                                                                     |
| ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- |
| `meta`                                                                          | [operations.GetAccountMeta](../../models/operations/get-account-meta.md)        | :heavy_minus_sign:                                                              | N/A                                                                             |
| `data`                                                                          | [models.AccountResponseDto](../../models/account-response-dto.md)               | :heavy_check_mark:                                                              | N/A                                                                             |
| `errors`                                                                        | [operations.GetAccountErrors](../../models/operations/get-account-errors.md)    | :heavy_check_mark:                                                              | N/A                                                                             |
| `rawData`                                                                       | [operations.GetAccountRawData](../../models/operations/get-account-raw-data.md) | :heavy_check_mark:                                                              | N/A                                                                             |