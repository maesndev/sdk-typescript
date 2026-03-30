# GetAccountsResponse

List of accounts for the authenticated end user's connected target system

## Example Usage

```typescript
import { GetAccountsResponse } from "@maesn/typescript-sdk/models/operations";

let value: GetAccountsResponse = {
  data: [],
  errors: {},
  rawData: {},
};
```

## Fields

| Field                                                                             | Type                                                                              | Required                                                                          | Description                                                                       |
| --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- |
| `meta`                                                                            | [operations.GetAccountsMeta](../../models/operations/get-accounts-meta.md)        | :heavy_minus_sign:                                                                | N/A                                                                               |
| `data`                                                                            | [models.AccountResponseDto](../../models/account-response-dto.md)[]               | :heavy_check_mark:                                                                | N/A                                                                               |
| `errors`                                                                          | [operations.GetAccountsErrors](../../models/operations/get-accounts-errors.md)    | :heavy_check_mark:                                                                | N/A                                                                               |
| `rawData`                                                                         | [operations.GetAccountsRawData](../../models/operations/get-accounts-raw-data.md) | :heavy_check_mark:                                                                | N/A                                                                               |