# GetBillsRequest

## Example Usage

```typescript
import { GetBillsRequest } from "maesn/models/operations";

let value: GetBillsRequest = {};
```

## Fields

| Field                                                                                   | Type                                                                                    | Required                                                                                | Description                                                                             |
| --------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------- |
| `page`                                                                                  | *number*                                                                                | :heavy_minus_sign:                                                                      | N/A                                                                                     |
| `limit`                                                                                 | *number*                                                                                | :heavy_minus_sign:                                                                      | N/A                                                                                     |
| `lastModifiedAt`                                                                        | *string*                                                                                | :heavy_minus_sign:                                                                      | N/A                                                                                     |
| `environmentName`                                                                       | *string*                                                                                | :heavy_minus_sign:                                                                      | N/A                                                                                     |
| `companyId`                                                                             | *string*                                                                                | :heavy_minus_sign:                                                                      | N/A                                                                                     |
| `status`                                                                                | [operations.GetBillsStatus](../../models/operations/get-bills-status.md)                | :heavy_minus_sign:                                                                      | N/A                                                                                     |
| `paymentStatus`                                                                         | [operations.GetBillsPaymentStatus](../../models/operations/get-bills-payment-status.md) | :heavy_minus_sign:                                                                      | N/A                                                                                     |
| `rawData`                                                                               | *boolean*                                                                               | :heavy_minus_sign:                                                                      | N/A                                                                                     |
| `orderField`                                                                            | [operations.GetBillsOrderField](../../models/operations/get-bills-order-field.md)       | :heavy_minus_sign:                                                                      | N/A                                                                                     |
| `orderDir`                                                                              | [operations.GetBillsOrderDir](../../models/operations/get-bills-order-dir.md)           | :heavy_minus_sign:                                                                      | N/A                                                                                     |