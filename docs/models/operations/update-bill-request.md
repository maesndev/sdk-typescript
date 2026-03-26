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

| Field                                                                  | Type                                                                   | Required                                                               | Description                                                            |
| ---------------------------------------------------------------------- | ---------------------------------------------------------------------- | ---------------------------------------------------------------------- | ---------------------------------------------------------------------- |
| `billId`                                                               | *string*                                                               | :heavy_check_mark:                                                     | N/A                                                                    |
| `environmentName`                                                      | *string*                                                               | :heavy_minus_sign:                                                     | N/A                                                                    |
| `companyId`                                                            | *string*                                                               | :heavy_minus_sign:                                                     | N/A                                                                    |
| `body`                                                                 | [models.CreateBillRequestDto](../../models/create-bill-request-dto.md) | :heavy_check_mark:                                                     | N/A                                                                    |