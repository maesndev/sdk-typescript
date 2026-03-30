# CreatePaymentResponse

Payment created successfully

## Example Usage

```typescript
import { CreatePaymentResponse } from "@maesn/typescript-sdk/models/operations";

let value: CreatePaymentResponse = {
  data: {
    id: "<id>",
    currency: "Kenyan Shilling",
    createdDate: "<value>",
    documentType: "BILL",
    exchangeRate: 7650.33,
    journalCode: "<value>",
    updatedDate: null,
    paymentType: null,
    paymentLines: [
      {
        accountId: "<id>",
        amount: 5456.15,
        contactName: "<value>",
        description: "up ew productive",
        invoiceId: "<id>",
        supplierId: "<id>",
        paymentDate: "<value>",
      },
    ],
  },
  errors: {},
  rawData: null,
};
```

## Fields

| Field                                                                                 | Type                                                                                  | Required                                                                              | Description                                                                           |
| ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- |
| `meta`                                                                                | [operations.CreatePaymentMeta](../../models/operations/create-payment-meta.md)        | :heavy_minus_sign:                                                                    | N/A                                                                                   |
| `data`                                                                                | [models.PaymentResponseDto](../../models/payment-response-dto.md)                     | :heavy_check_mark:                                                                    | N/A                                                                                   |
| `errors`                                                                              | [operations.CreatePaymentErrors](../../models/operations/create-payment-errors.md)    | :heavy_check_mark:                                                                    | N/A                                                                                   |
| `rawData`                                                                             | [operations.CreatePaymentRawData](../../models/operations/create-payment-raw-data.md) | :heavy_check_mark:                                                                    | N/A                                                                                   |