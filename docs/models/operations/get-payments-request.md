# GetPaymentsRequest

## Example Usage

```typescript
import { GetPaymentsRequest } from "@maesn/typescript-sdk/models/operations";

let value: GetPaymentsRequest = {};
```

## Fields

| Field                                                                              | Type                                                                               | Required                                                                           | Description                                                                        |
| ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- |
| `page`                                                                             | *number*                                                                           | :heavy_minus_sign:                                                                 | N/A                                                                                |
| `limit`                                                                            | [operations.GetPaymentsLimit](../../models/operations/get-payments-limit.md)       | :heavy_minus_sign:                                                                 | N/A                                                                                |
| `environmentName`                                                                  | *string*                                                                           | :heavy_minus_sign:                                                                 | Environment name (required for multi-environment systems such as Business Central) |
| `companyId`                                                                        | *string*                                                                           | :heavy_minus_sign:                                                                 | ID of the company (required for multi-company target systems)                      |
| `lastModifiedAt`                                                                   | *string*                                                                           | :heavy_minus_sign:                                                                 | ISO 8601 timestamp; only records modified after this date are returned             |
| `invoiceId`                                                                        | *string*                                                                           | :heavy_minus_sign:                                                                 | ID of the invoice to filter payments by                                            |
| `rawData`                                                                          | *boolean*                                                                          | :heavy_minus_sign:                                                                 | When true, returns the unprocessed response from the upstream target system        |
| `apiKey`                                                                           | *string*                                                                           | :heavy_minus_sign:                                                                 | API key                                                                            |
| `accountKey`                                                                       | *string*                                                                           | :heavy_minus_sign:                                                                 | Account key                                                                        |