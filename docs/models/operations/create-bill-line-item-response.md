# CreateBillLineItemResponse

Bill line item created successfully

## Example Usage

```typescript
import { CreateBillLineItemResponse } from "@maesn/typescript-sdk/models/operations";

let value: CreateBillLineItemResponse = {
  data: [],
  errors: {},
  rawData: {},
};
```

## Fields

| Field                                                                                             | Type                                                                                              | Required                                                                                          | Description                                                                                       |
| ------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------- |
| `meta`                                                                                            | [operations.CreateBillLineItemMeta](../../models/operations/create-bill-line-item-meta.md)        | :heavy_minus_sign:                                                                                | N/A                                                                                               |
| `data`                                                                                            | [models.BillLineItemResponseDto](../../models/bill-line-item-response-dto.md)[]                   | :heavy_check_mark:                                                                                | N/A                                                                                               |
| `errors`                                                                                          | [operations.CreateBillLineItemErrors](../../models/operations/create-bill-line-item-errors.md)    | :heavy_check_mark:                                                                                | N/A                                                                                               |
| `rawData`                                                                                         | [operations.CreateBillLineItemRawData](../../models/operations/create-bill-line-item-raw-data.md) | :heavy_check_mark:                                                                                | N/A                                                                                               |