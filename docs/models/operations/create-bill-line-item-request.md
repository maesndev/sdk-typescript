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
| `companyId`                                                                              | *string*                                                                                 | :heavy_minus_sign:                                                                       | ID of the company (required for multi-company target systems)                            |
| `apiKey`                                                                                 | *string*                                                                                 | :heavy_minus_sign:                                                                       | API key                                                                                  |
| `accountKey`                                                                             | *string*                                                                                 | :heavy_minus_sign:                                                                       | Account key                                                                              |
| `body`                                                                                   | [models.CreateBillLineItemRequestDto](../../models/create-bill-line-item-request-dto.md) | :heavy_check_mark:                                                                       | N/A                                                                                      |