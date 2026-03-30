# GetLineItemsResponse

List of line items for the authenticated end user's connected target system

## Example Usage

```typescript
import { GetLineItemsResponse } from "@maesn/typescript-sdk/models/operations";

let value: GetLineItemsResponse = {
  data: [
    {
      lineItemId: "<id>",
      accountId: "<id>",
      createdDate: "<value>",
      description: "so yuck perp phooey intent",
      dimensions: [],
      discountItemAmount: null,
      discountItemPercentage: 9973.62,
      grossAmount: 6692.06,
      itemsAmount: 3109.42,
      itemId: "<id>",
      name: null,
      quantity: 1681.48,
      taxRatePercentage: 2840.68,
      unitAmount: 6368.56,
      updatedDate: "<value>",
    },
  ],
  errors: {},
  rawData: {},
};
```

## Fields

| Field                                                                                | Type                                                                                 | Required                                                                             | Description                                                                          |
| ------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------ |
| `meta`                                                                               | [operations.GetLineItemsMeta](../../models/operations/get-line-items-meta.md)        | :heavy_minus_sign:                                                                   | N/A                                                                                  |
| `data`                                                                               | [models.LineItemResponseDto](../../models/line-item-response-dto.md)[]               | :heavy_check_mark:                                                                   | N/A                                                                                  |
| `errors`                                                                             | [operations.GetLineItemsErrors](../../models/operations/get-line-items-errors.md)    | :heavy_check_mark:                                                                   | N/A                                                                                  |
| `rawData`                                                                            | [operations.GetLineItemsRawData](../../models/operations/get-line-items-raw-data.md) | :heavy_check_mark:                                                                   | N/A                                                                                  |