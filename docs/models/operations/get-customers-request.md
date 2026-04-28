# GetCustomersRequest

## Example Usage

```typescript
import { GetCustomersRequest } from "@maesn/typescript-sdk/models/operations";

let value: GetCustomersRequest = {};
```

## Fields

| Field                                                                              | Type                                                                               | Required                                                                           | Description                                                                        |
| ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- |
| `page`                                                                             | *number*                                                                           | :heavy_minus_sign:                                                                 | N/A                                                                                |
| `limit`                                                                            | [operations.GetCustomersLimit](../../models/operations/get-customers-limit.md)     | :heavy_minus_sign:                                                                 | N/A                                                                                |
| `lastModifiedAt`                                                                   | *string*                                                                           | :heavy_minus_sign:                                                                 | ISO 8601 timestamp; only records modified after this date are returned             |
| `environmentName`                                                                  | *string*                                                                           | :heavy_minus_sign:                                                                 | Environment name (required for multi-environment systems such as Business Central) |
| `companyId`                                                                        | *string*                                                                           | :heavy_minus_sign:                                                                 | ID of the company (required for multi-company target systems)                      |
| `rawData`                                                                          | *boolean*                                                                          | :heavy_minus_sign:                                                                 | When true, returns the unprocessed response from the upstream target system        |
| `email`                                                                            | *string*                                                                           | :heavy_minus_sign:                                                                 | Filter customers by email address                                                  |
| `name`                                                                             | *string*                                                                           | :heavy_minus_sign:                                                                 | Filter customers by name                                                           |
| `number`                                                                           | *string*                                                                           | :heavy_minus_sign:                                                                 | Filter customers by customer number                                                |
| `apiKey`                                                                           | *string*                                                                           | :heavy_minus_sign:                                                                 | API key                                                                            |
| `accountKey`                                                                       | *string*                                                                           | :heavy_minus_sign:                                                                 | Account key                                                                        |