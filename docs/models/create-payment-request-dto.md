# CreatePaymentRequestDto

## Example Usage

```typescript
import { CreatePaymentRequestDto } from "maesn/models";

let value: CreatePaymentRequestDto = {
  currency: "New Taiwan Dollar",
  documentType: "<value>",
  exchangeRate: 3700.37,
  journalCode: "<value>",
  paymentType: "<value>",
  paymentLines: [
    {
      accountId: "<id>",
      amount: 3072.36,
      contactName: "<value>",
      customerId: "<id>",
      description: "construe ick reconstitute whoa",
      invoiceId: "<id>",
      supplierId: "<id>",
      paymentDate: "<value>",
    },
  ],
};
```

## Fields

| Field                                                          | Type                                                           | Required                                                       | Description                                                    |
| -------------------------------------------------------------- | -------------------------------------------------------------- | -------------------------------------------------------------- | -------------------------------------------------------------- |
| `currency`                                                     | *string*                                                       | :heavy_check_mark:                                             | N/A                                                            |
| `documentType`                                                 | *string*                                                       | :heavy_check_mark:                                             | N/A                                                            |
| `exchangeRate`                                                 | *number*                                                       | :heavy_check_mark:                                             | N/A                                                            |
| `journalCode`                                                  | *string*                                                       | :heavy_check_mark:                                             | N/A                                                            |
| `paymentType`                                                  | *string*                                                       | :heavy_check_mark:                                             | N/A                                                            |
| `paymentLines`                                                 | [models.CreatePaymentLine](../models/create-payment-line.md)[] | :heavy_check_mark:                                             | N/A                                                            |