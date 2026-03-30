# GetExpensesRequest

## Example Usage

```typescript
import { GetExpensesRequest } from "@maesn/typescript-sdk/models/operations";

let value: GetExpensesRequest = {};
```

## Fields

| Field                                                                       | Type                                                                        | Required                                                                    | Description                                                                 |
| --------------------------------------------------------------------------- | --------------------------------------------------------------------------- | --------------------------------------------------------------------------- | --------------------------------------------------------------------------- |
| `page`                                                                      | *number*                                                                    | :heavy_minus_sign:                                                          | N/A                                                                         |
| `limit`                                                                     | *number*                                                                    | :heavy_minus_sign:                                                          | N/A                                                                         |
| `lastModifiedAt`                                                            | *string*                                                                    | :heavy_minus_sign:                                                          | ISO 8601 timestamp; only records modified after this date are returned      |
| `companyId`                                                                 | *string*                                                                    | :heavy_minus_sign:                                                          | ID of the company (required for multi-company target systems)               |
| `rawData`                                                                   | *boolean*                                                                   | :heavy_minus_sign:                                                          | When true, returns the unprocessed response from the upstream target system |