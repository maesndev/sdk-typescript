# PaymentResponseDto

## Example Usage

```typescript
import { PaymentResponseDto } from "maesn/models";

let value: PaymentResponseDto = {
  id: "<id>",
  currency: "Barbados Dollar",
  createdDate: "<value>",
  documentType: "<value>",
  exchangeRate: 3549.14,
  journalCode: "<value>",
  updatedDate: "<value>",
  paymentType: "<value>",
  paymentLines: [
    {
      accountId: "<id>",
      amount: 8330.75,
      contactName: "<value>",
      customerId: "<id>",
      description: "beyond bleakly geez sunder even once",
      invoiceId: "<id>",
      supplierId: "<id>",
      paymentDate: "<value>",
    },
  ],
};
```

## Fields

| Field                                             | Type                                              | Required                                          | Description                                       |
| ------------------------------------------------- | ------------------------------------------------- | ------------------------------------------------- | ------------------------------------------------- |
| `id`                                              | *string*                                          | :heavy_check_mark:                                | N/A                                               |
| `currency`                                        | *string*                                          | :heavy_check_mark:                                | N/A                                               |
| `createdDate`                                     | *string*                                          | :heavy_check_mark:                                | N/A                                               |
| `documentType`                                    | *string*                                          | :heavy_check_mark:                                | N/A                                               |
| `exchangeRate`                                    | *number*                                          | :heavy_check_mark:                                | N/A                                               |
| `journalCode`                                     | *string*                                          | :heavy_check_mark:                                | N/A                                               |
| `updatedDate`                                     | *string*                                          | :heavy_check_mark:                                | N/A                                               |
| `paymentType`                                     | *string*                                          | :heavy_check_mark:                                | N/A                                               |
| `paymentLines`                                    | [models.PaymentLine](../models/payment-line.md)[] | :heavy_check_mark:                                | N/A                                               |