# GetAccountsResponse

## Example Usage

```typescript
import { GetAccountsResponse } from "maesn/models/operations";

let value: GetAccountsResponse = {
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
  data: [],
  errors: {},
  rawData: {},
};
```

## Fields

| Field                                                                             | Type                                                                              | Required                                                                          | Description                                                                       |
| --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- |
| `meta`                                                                            | [models.MetaResponse](../../models/meta-response.md)                              | :heavy_check_mark:                                                                | N/A                                                                               |
| `data`                                                                            | [models.AccountResponseDto](../../models/account-response-dto.md)[]               | :heavy_check_mark:                                                                | N/A                                                                               |
| `errors`                                                                          | [operations.GetAccountsErrors](../../models/operations/get-accounts-errors.md)    | :heavy_check_mark:                                                                | N/A                                                                               |
| `rawData`                                                                         | [operations.GetAccountsRawData](../../models/operations/get-accounts-raw-data.md) | :heavy_check_mark:                                                                | N/A                                                                               |