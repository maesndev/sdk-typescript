# GetPurchaseOrdersResponse

List of purchase orders for the authenticated end user's connected target system

## Example Usage

```typescript
import { GetPurchaseOrdersResponse } from "@maesn/typescript-sdk/models/operations";

let value: GetPurchaseOrdersResponse = {
  data: [],
  errors: {},
  rawData: {},
};
```

## Fields

| Field                                                                                          | Type                                                                                           | Required                                                                                       | Description                                                                                    |
| ---------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------- |
| `meta`                                                                                         | [operations.GetPurchaseOrdersMeta](../../models/operations/get-purchase-orders-meta.md)        | :heavy_minus_sign:                                                                             | N/A                                                                                            |
| `data`                                                                                         | [models.PurchaseOrderResponseDto](../../models/purchase-order-response-dto.md)[]               | :heavy_check_mark:                                                                             | N/A                                                                                            |
| `errors`                                                                                       | [operations.GetPurchaseOrdersErrors](../../models/operations/get-purchase-orders-errors.md)    | :heavy_check_mark:                                                                             | N/A                                                                                            |
| `rawData`                                                                                      | [operations.GetPurchaseOrdersRawData](../../models/operations/get-purchase-orders-raw-data.md) | :heavy_check_mark:                                                                             | N/A                                                                                            |