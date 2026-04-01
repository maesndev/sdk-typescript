# GetSuppliersRequest

## Example Usage

```typescript
import { GetSuppliersRequest } from "@maesn/typescript-sdk/models/operations";

let value: GetSuppliersRequest = {};
```

## Fields

| Field                                                                              | Type                                                                               | Required                                                                           | Description                                                                        |
| ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- |
| `page`                                                                             | *number*                                                                           | :heavy_minus_sign:                                                                 | N/A                                                                                |
| `limit`                                                                            | [operations.GetSuppliersLimit](../../models/operations/get-suppliers-limit.md)     | :heavy_minus_sign:                                                                 | N/A                                                                                |
| `lastModifiedAt`                                                                   | *string*                                                                           | :heavy_minus_sign:                                                                 | ISO 8601 timestamp; only records modified after this date are returned             |
| `environmentName`                                                                  | *string*                                                                           | :heavy_minus_sign:                                                                 | Environment name (required for multi-environment systems such as Business Central) |
| `companyId`                                                                        | *string*                                                                           | :heavy_minus_sign:                                                                 | ID of the company (required for multi-company target systems)                      |
| `rawData`                                                                          | *boolean*                                                                          | :heavy_minus_sign:                                                                 | When true, returns the unprocessed response from the upstream target system        |
| `email`                                                                            | *string*                                                                           | :heavy_minus_sign:                                                                 | Filter suppliers by email address                                                  |
| `name`                                                                             | *string*                                                                           | :heavy_minus_sign:                                                                 | Filter suppliers by name                                                           |
| `number`                                                                           | *string*                                                                           | :heavy_minus_sign:                                                                 | Filter suppliers by supplier number                                                |