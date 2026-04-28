# GetOffersRequest

## Example Usage

```typescript
import { GetOffersRequest } from "@maesn/typescript-sdk/models/operations";

let value: GetOffersRequest = {};
```

## Fields

| Field                                                                              | Type                                                                               | Required                                                                           | Description                                                                        |
| ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- |
| `page`                                                                             | *number*                                                                           | :heavy_minus_sign:                                                                 | N/A                                                                                |
| `limit`                                                                            | [operations.GetOffersLimit](../../models/operations/get-offers-limit.md)           | :heavy_minus_sign:                                                                 | N/A                                                                                |
| `lastModifiedAt`                                                                   | *string*                                                                           | :heavy_minus_sign:                                                                 | ISO 8601 timestamp; only records modified after this date are returned             |
| `environmentName`                                                                  | *string*                                                                           | :heavy_minus_sign:                                                                 | Environment name (required for multi-environment systems such as Business Central) |
| `companyId`                                                                        | *string*                                                                           | :heavy_minus_sign:                                                                 | ID of the company (required for multi-company target systems)                      |
| `status`                                                                           | [operations.GetOffersStatus](../../models/operations/get-offers-status.md)         | :heavy_minus_sign:                                                                 | Filter offers by unified status                                                    |
| `rawData`                                                                          | *boolean*                                                                          | :heavy_minus_sign:                                                                 | When true, returns the unprocessed response from the upstream target system        |
| `apiKey`                                                                           | *string*                                                                           | :heavy_minus_sign:                                                                 | API key                                                                            |
| `accountKey`                                                                       | *string*                                                                           | :heavy_minus_sign:                                                                 | Account key                                                                        |