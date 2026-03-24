# CreditNoteResponseDto

## Example Usage

```typescript
import { CreditNoteResponseDto } from "maesn/models";

let value: CreditNoteResponseDto = {
  id: "<id>",
  addresses: [],
  contactId: "<id>",
  createdDate: "<value>",
  creditNoteDate: "<value>",
  creditNoteLines: [
    {
      id: "<id>",
      createdDate: "<value>",
      description: "segregate whoever decision nudge whose fragrant even",
      itemId: "<id>",
      itemName: "<value>",
      quantity: 2003.9,
      taxCode: "<value>",
      taxRatePercentage: 8902.42,
      totalDiscountAmount: 3033.59,
      totalDiscountPercentage: 9674.25,
      totalGrossAmount: 9006.47,
      totalNetAmount: 2669.72,
      totalTaxAmount: 815.48,
      unitAmount: 8447.51,
      unitDiscountAmount: 9784.31,
      unitDiscountPercentage: 8251.52,
      unitName: "<value>",
      updatedDate: "<value>",
    },
  ],
  creditNoteNumber: "<value>",
  currency: "Colombian Peso",
  paymentStatus: "PARTIAL_CANCELLATION",
  paymentTermId: "<id>",
  reference: "<value>",
  status: "PAID",
  totalDiscountAmount: 3538.3,
  totalDiscountPercentage: 7777.6,
  totalGrossAmount: 392.99,
  totalNetAmount: 8571.57,
  totalTaxAmount: 1524.63,
  updatedDate: "<value>",
};
```

## Fields

| Field                                                                                             | Type                                                                                              | Required                                                                                          | Description                                                                                       |
| ------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------- |
| `id`                                                                                              | *string*                                                                                          | :heavy_check_mark:                                                                                | N/A                                                                                               |
| `addresses`                                                                                       | [models.Address](../models/address.md)[]                                                          | :heavy_check_mark:                                                                                | N/A                                                                                               |
| `contactId`                                                                                       | *string*                                                                                          | :heavy_check_mark:                                                                                | N/A                                                                                               |
| `createdDate`                                                                                     | *string*                                                                                          | :heavy_check_mark:                                                                                | N/A                                                                                               |
| `creditNoteDate`                                                                                  | *string*                                                                                          | :heavy_check_mark:                                                                                | N/A                                                                                               |
| `creditNoteLines`                                                                                 | [models.CreditNoteLinesDto](../models/credit-note-lines-dto.md)[]                                 | :heavy_check_mark:                                                                                | N/A                                                                                               |
| `creditNoteNumber`                                                                                | *string*                                                                                          | :heavy_check_mark:                                                                                | N/A                                                                                               |
| `currency`                                                                                        | *string*                                                                                          | :heavy_check_mark:                                                                                | N/A                                                                                               |
| `paymentStatus`                                                                                   | [models.CreditNoteResponseDtoPaymentStatus](../models/credit-note-response-dto-payment-status.md) | :heavy_check_mark:                                                                                | N/A                                                                                               |
| `paymentTermId`                                                                                   | *string*                                                                                          | :heavy_check_mark:                                                                                | N/A                                                                                               |
| `reference`                                                                                       | *string*                                                                                          | :heavy_check_mark:                                                                                | N/A                                                                                               |
| `status`                                                                                          | [models.CreditNoteResponseDtoStatus](../models/credit-note-response-dto-status.md)                | :heavy_check_mark:                                                                                | N/A                                                                                               |
| `totalDiscountAmount`                                                                             | *number*                                                                                          | :heavy_check_mark:                                                                                | N/A                                                                                               |
| `totalDiscountPercentage`                                                                         | *number*                                                                                          | :heavy_check_mark:                                                                                | N/A                                                                                               |
| `totalGrossAmount`                                                                                | *number*                                                                                          | :heavy_check_mark:                                                                                | N/A                                                                                               |
| `totalNetAmount`                                                                                  | *number*                                                                                          | :heavy_check_mark:                                                                                | N/A                                                                                               |
| `totalTaxAmount`                                                                                  | *number*                                                                                          | :heavy_check_mark:                                                                                | N/A                                                                                               |
| `updatedDate`                                                                                     | *string*                                                                                          | :heavy_check_mark:                                                                                | N/A                                                                                               |