# GetOpenItemsRequest

## Example Usage

```typescript
import { GetOpenItemsRequest } from "@maesn/typescript-sdk/models/operations";

let value: GetOpenItemsRequest = {};
```

## Fields

| Field                                                                              | Type                                                                               | Required                                                                           | Description                                                                        |
| ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- |
| `page`                                                                             | *number*                                                                           | :heavy_minus_sign:                                                                 | N/A                                                                                |
| `limit`                                                                            | [operations.GetOpenItemsLimit](../../models/operations/get-open-items-limit.md)    | :heavy_minus_sign:                                                                 | N/A                                                                                |
| `lastModifiedAt`                                                                   | *string*                                                                           | :heavy_minus_sign:                                                                 | ISO 8601 timestamp; only records modified after this date are returned             |
| `environmentName`                                                                  | *string*                                                                           | :heavy_minus_sign:                                                                 | Environment name (required for multi-environment systems such as Business Central) |
| `companyId`                                                                        | *string*                                                                           | :heavy_minus_sign:                                                                 | ID of the company (required for multi-company target systems)                      |
| `rawData`                                                                          | *boolean*                                                                          | :heavy_minus_sign:                                                                 | When true, returns the unprocessed response from the upstream target system        |
| `fiscalYear`                                                                       | *number*                                                                           | :heavy_minus_sign:                                                                 | Fiscal year to scope the open items results (e.g. 2024)                            |
| `accountNumber`                                                                    | *string*                                                                           | :heavy_minus_sign:                                                                 | Filter open items by account number                                                |
| `documentNumber`                                                                   | *string*                                                                           | :heavy_minus_sign:                                                                 | Filter open items by document number                                               |
| `type`                                                                             | *string*                                                                           | :heavy_minus_sign:                                                                 | Filter open items by type (e.g. receivable, payable)                               |
| `apiKey`                                                                           | *string*                                                                           | :heavy_minus_sign:                                                                 | API key                                                                            |
| `accountKey`                                                                       | *string*                                                                           | :heavy_minus_sign:                                                                 | Account key                                                                        |