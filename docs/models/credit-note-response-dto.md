# CreditNoteResponseDto

## Example Usage

```typescript
import { CreditNoteResponseDto } from "@maesn/typescript-sdk/models";

let value: CreditNoteResponseDto = {
  id: null,
  addresses: [
    {},
  ],
  contactId: "<id>",
  createdDate: "<value>",
  creditNoteDate: "<value>",
  creditNoteLines: [],
  creditNoteNumber: null,
  currency: "Danish Krone",
  paymentStatus: "CANCELED",
  paymentTermId: "<id>",
  reference: "<value>",
  status: "VOIDED",
  totalDiscountAmount: 9899.06,
  totalDiscountPercentage: 3957.71,
  totalGrossAmount: 5304.94,
  totalNetAmount: 1831.02,
  totalTaxAmount: 7011.77,
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