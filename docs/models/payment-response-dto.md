# PaymentResponseDto

## Example Usage

```typescript
import { PaymentResponseDto } from "@maesn/typescript-sdk/models";

let value: PaymentResponseDto = {
  id: null,
  currency: "New Zealand Dollar",
  createdDate: "<value>",
  description: "above rarely mozzarella",
  documentType: "INVOICE_BOOKING_PROPOSAL",
  exchangeRate: 6921.61,
  journalId: "<id>",
  journalCode: "<value>",
  updatedDate: "<value>",
  paymentDate: null,
  paymentType: "<value>",
  paymentLines: [],
};
```

## Fields

| Field                                                                                    | Type                                                                                     | Required                                                                                 | Description                                                                              |
| ---------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------- |
| `id`                                                                                     | *string*                                                                                 | :heavy_check_mark:                                                                       | N/A                                                                                      |
| `currency`                                                                               | *string*                                                                                 | :heavy_check_mark:                                                                       | N/A                                                                                      |
| `createdDate`                                                                            | *string*                                                                                 | :heavy_check_mark:                                                                       | N/A                                                                                      |
| `description`                                                                            | *string*                                                                                 | :heavy_check_mark:                                                                       | N/A                                                                                      |
| `documentType`                                                                           | [models.PaymentResponseDtoDocumentType](../models/payment-response-dto-document-type.md) | :heavy_check_mark:                                                                       | N/A                                                                                      |
| `exchangeRate`                                                                           | *number*                                                                                 | :heavy_check_mark:                                                                       | N/A                                                                                      |
| `journalId`                                                                              | *string*                                                                                 | :heavy_check_mark:                                                                       | N/A                                                                                      |
| `journalCode`                                                                            | *string*                                                                                 | :heavy_check_mark:                                                                       | N/A                                                                                      |
| `updatedDate`                                                                            | *string*                                                                                 | :heavy_check_mark:                                                                       | N/A                                                                                      |
| `paymentDate`                                                                            | *string*                                                                                 | :heavy_check_mark:                                                                       | N/A                                                                                      |
| `paymentType`                                                                            | *string*                                                                                 | :heavy_check_mark:                                                                       | N/A                                                                                      |
| `paymentLines`                                                                           | [models.PaymentLine](../models/payment-line.md)[]                                        | :heavy_check_mark:                                                                       | N/A                                                                                      |