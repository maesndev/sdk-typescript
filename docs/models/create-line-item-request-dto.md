# CreateLineItemRequestDto

## Example Usage

```typescript
import { CreateLineItemRequestDto } from "@maesn/typescript-sdk/models";

let value: CreateLineItemRequestDto = {
  quantity: 4687.34,
};
```

## Fields

| Field                                                                             | Type                                                                              | Required                                                                          | Description                                                                       |
| --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- |
| `accountCode`                                                                     | *string*                                                                          | :heavy_minus_sign:                                                                | N/A                                                                               |
| `accountId`                                                                       | *string*                                                                          | :heavy_minus_sign:                                                                | N/A                                                                               |
| `description`                                                                     | *string*                                                                          | :heavy_minus_sign:                                                                | N/A                                                                               |
| `dimensions`                                                                      | [models.InvoiceDimensionRequestDto](../models/invoice-dimension-request-dto.md)[] | :heavy_minus_sign:                                                                | N/A                                                                               |
| `discountItemPercentage`                                                          | *number*                                                                          | :heavy_minus_sign:                                                                | N/A                                                                               |
| `grossAmount`                                                                     | *number*                                                                          | :heavy_minus_sign:                                                                | N/A                                                                               |
| `itemId`                                                                          | *string*                                                                          | :heavy_minus_sign:                                                                | N/A                                                                               |
| `name`                                                                            | *string*                                                                          | :heavy_minus_sign:                                                                | N/A                                                                               |
| `quantity`                                                                        | *number*                                                                          | :heavy_check_mark:                                                                | N/A                                                                               |
| `taxCode`                                                                         | *string*                                                                          | :heavy_minus_sign:                                                                | N/A                                                                               |
| `taxRatePercentage`                                                               | *number*                                                                          | :heavy_minus_sign:                                                                | N/A                                                                               |
| `taxType`                                                                         | *string*                                                                          | :heavy_minus_sign:                                                                | N/A                                                                               |
| `type`                                                                            | *string*                                                                          | :heavy_minus_sign:                                                                | N/A                                                                               |
| `unitAmount`                                                                      | *number*                                                                          | :heavy_minus_sign:                                                                | N/A                                                                               |
| `unitName`                                                                        | *string*                                                                          | :heavy_minus_sign:                                                                | N/A                                                                               |