# GetBankAccountsRequest

## Example Usage

```typescript
import { GetBankAccountsRequest } from "@maesn/typescript-sdk/models/operations";

let value: GetBankAccountsRequest = {};
```

## Fields

| Field                                                                                 | Type                                                                                  | Required                                                                              | Description                                                                           |
| ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- |
| `page`                                                                                | *number*                                                                              | :heavy_minus_sign:                                                                    | N/A                                                                                   |
| `limit`                                                                               | [operations.GetBankAccountsLimit](../../models/operations/get-bank-accounts-limit.md) | :heavy_minus_sign:                                                                    | N/A                                                                                   |
| `lastModifiedAt`                                                                      | *string*                                                                              | :heavy_minus_sign:                                                                    | ISO 8601 timestamp; only records modified after this date are returned                |
| `environmentName`                                                                     | *string*                                                                              | :heavy_minus_sign:                                                                    | Environment name (required for multi-environment systems such as Business Central)    |
| `companyId`                                                                           | *string*                                                                              | :heavy_minus_sign:                                                                    | ID of the company (required for multi-company target systems)                         |
| `rawData`                                                                             | *boolean*                                                                             | :heavy_minus_sign:                                                                    | When true, returns the unprocessed response from the upstream target system           |
| `apiKey`                                                                              | *string*                                                                              | :heavy_minus_sign:                                                                    | API key                                                                               |
| `accountKey`                                                                          | *string*                                                                              | :heavy_minus_sign:                                                                    | Account key                                                                           |