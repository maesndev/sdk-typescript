# CreateBillLineItemRequest

## Example Usage

```typescript
import { CreateBillLineItemRequest } from "@maesn/typescript-sdk/models/operations";

let value: CreateBillLineItemRequest = {
  billId: "<id>",
  body: {},
};
```

## Fields

| Field                                                                                    | Type                                                                                     | Required                                                                                 | Description                                                                              |
| ---------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------- |
| `billId`                                                                                 | *string*                                                                                 | :heavy_check_mark:                                                                       | N/A                                                                                      |
| `companyId`                                                                              | *string*                                                                                 | :heavy_minus_sign:                                                                       | N/A                                                                                      |
| `body`                                                                                   | [models.CreateBillLineItemRequestDto](../../models/create-bill-line-item-request-dto.md) | :heavy_check_mark:                                                                       | N/A                                                                                      |