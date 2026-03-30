# GetSalesOrdersResponse

List of sales orders for the authenticated end user's connected target system

## Example Usage

```typescript
import { GetSalesOrdersResponse } from "@maesn/typescript-sdk/models/operations";

let value: GetSalesOrdersResponse = {
  data: [],
  errors: {},
  rawData: {},
};
```

## Fields

| Field                                                                                    | Type                                                                                     | Required                                                                                 | Description                                                                              |
| ---------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------- |
| `meta`                                                                                   | [operations.GetSalesOrdersMeta](../../models/operations/get-sales-orders-meta.md)        | :heavy_minus_sign:                                                                       | N/A                                                                                      |
| `data`                                                                                   | [models.SalesOrderResponseDto](../../models/sales-order-response-dto.md)[]               | :heavy_check_mark:                                                                       | N/A                                                                                      |
| `errors`                                                                                 | [operations.GetSalesOrdersErrors](../../models/operations/get-sales-orders-errors.md)    | :heavy_check_mark:                                                                       | N/A                                                                                      |
| `rawData`                                                                                | [operations.GetSalesOrdersRawData](../../models/operations/get-sales-orders-raw-data.md) | :heavy_check_mark:                                                                       | N/A                                                                                      |