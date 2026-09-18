# GetOpenItemsAsyncRequest

## Example Usage

```typescript
import { GetOpenItemsAsyncRequest } from "@maesn/typescript-sdk/models/operations";

let value: GetOpenItemsAsyncRequest = {};
```

## Fields

| Field                                                                                      | Type                                                                                       | Required                                                                                   | Description                                                                                |
| ------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------ |
| `page`                                                                                     | *number*                                                                                   | :heavy_minus_sign:                                                                         | N/A                                                                                        |
| `limit`                                                                                    | [operations.GetOpenItemsAsyncLimit](../../models/operations/get-open-items-async-limit.md) | :heavy_minus_sign:                                                                         | N/A                                                                                        |
| `environmentName`                                                                          | *string*                                                                                   | :heavy_minus_sign:                                                                         | Environment name (required for multi-environment systems such as Business Central)         |
| `companyId`                                                                                | *string*                                                                                   | :heavy_minus_sign:                                                                         | ID of the company (required for multi-company target systems)                              |
| `rawData`                                                                                  | *boolean*                                                                                  | :heavy_minus_sign:                                                                         | When true, returns the unprocessed response from the upstream target system                |
| `fiscalYearStartDate`                                                                      | *string*                                                                                   | :heavy_minus_sign:                                                                         | ISO 8601 start date of the fiscal year used for balance calculation                        |
| `apiKey`                                                                                   | *string*                                                                                   | :heavy_minus_sign:                                                                         | API key                                                                                    |
| `accountKey`                                                                               | *string*                                                                                   | :heavy_minus_sign:                                                                         | Account key                                                                                |