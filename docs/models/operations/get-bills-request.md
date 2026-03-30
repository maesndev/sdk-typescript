# GetBillsRequest

## Example Usage

```typescript
import { GetBillsRequest } from "@maesn/typescript-sdk/models/operations";

let value: GetBillsRequest = {};
```

## Fields

| Field                                                                                   | Type                                                                                    | Required                                                                                | Description                                                                             |
| --------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------- |
| `page`                                                                                  | *number*                                                                                | :heavy_minus_sign:                                                                      | N/A                                                                                     |
| `limit`                                                                                 | *number*                                                                                | :heavy_minus_sign:                                                                      | N/A                                                                                     |
| `lastModifiedAt`                                                                        | *string*                                                                                | :heavy_minus_sign:                                                                      | ISO 8601 timestamp; only records modified after this date are returned                  |
| `environmentName`                                                                       | *string*                                                                                | :heavy_minus_sign:                                                                      | Environment name (required for multi-environment systems such as Business Central)      |
| `companyId`                                                                             | *string*                                                                                | :heavy_minus_sign:                                                                      | ID of the company (required for multi-company target systems)                           |
| `status`                                                                                | [operations.GetBillsStatus](../../models/operations/get-bills-status.md)                | :heavy_minus_sign:                                                                      | Filter bills by unified status                                                          |
| `paymentStatus`                                                                         | [operations.GetBillsPaymentStatus](../../models/operations/get-bills-payment-status.md) | :heavy_minus_sign:                                                                      | Filter bills by payment status                                                          |
| `rawData`                                                                               | *boolean*                                                                               | :heavy_minus_sign:                                                                      | When true, returns the unprocessed response from the upstream target system             |
| `orderField`                                                                            | [operations.GetBillsOrderField](../../models/operations/get-bills-order-field.md)       | :heavy_minus_sign:                                                                      | Field to sort the results by                                                            |
| `orderDir`                                                                              | [operations.GetBillsOrderDir](../../models/operations/get-bills-order-dir.md)           | :heavy_minus_sign:                                                                      | Sort direction for the ordered results                                                  |