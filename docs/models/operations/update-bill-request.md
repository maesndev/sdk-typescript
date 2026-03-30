# UpdateBillRequest

## Example Usage

```typescript
import { UpdateBillRequest } from "@maesn/typescript-sdk/models/operations";

let value: UpdateBillRequest = {
  billId: "<id>",
  body: {},
};
```

## Fields

| Field                                                                              | Type                                                                               | Required                                                                           | Description                                                                        |
| ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- |
| `billId`                                                                           | *string*                                                                           | :heavy_check_mark:                                                                 | N/A                                                                                |
| `environmentName`                                                                  | *string*                                                                           | :heavy_minus_sign:                                                                 | Environment name (required for multi-environment systems such as Business Central) |
| `companyId`                                                                        | *string*                                                                           | :heavy_minus_sign:                                                                 | ID of the company (required for multi-company target systems)                      |
| `body`                                                                             | [models.CreateBillRequestDto](../../models/create-bill-request-dto.md)             | :heavy_check_mark:                                                                 | N/A                                                                                |