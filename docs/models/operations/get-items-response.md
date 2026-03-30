# GetItemsResponse

List of items for the authenticated end user's connected target system

## Example Usage

```typescript
import { GetItemsResponse } from "@maesn/typescript-sdk/models/operations";

let value: GetItemsResponse = {
  data: [],
  errors: null,
  rawData: {},
};
```

## Fields

| Field                                                                       | Type                                                                        | Required                                                                    | Description                                                                 |
| --------------------------------------------------------------------------- | --------------------------------------------------------------------------- | --------------------------------------------------------------------------- | --------------------------------------------------------------------------- |
| `meta`                                                                      | [operations.GetItemsMeta](../../models/operations/get-items-meta.md)        | :heavy_minus_sign:                                                          | N/A                                                                         |
| `data`                                                                      | [models.ItemResponseDto](../../models/item-response-dto.md)[]               | :heavy_check_mark:                                                          | N/A                                                                         |
| `errors`                                                                    | [operations.GetItemsErrors](../../models/operations/get-items-errors.md)    | :heavy_check_mark:                                                          | N/A                                                                         |
| `rawData`                                                                   | [operations.GetItemsRawData](../../models/operations/get-items-raw-data.md) | :heavy_check_mark:                                                          | N/A                                                                         |