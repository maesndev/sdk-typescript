# GetPaymentResponse

Payment record matching the provided ID

## Example Usage

```typescript
import { GetPaymentResponse } from "@maesn/typescript-sdk/models/operations";

let value: GetPaymentResponse = {
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

| Field                                                                           | Type                                                                            | Required                                                                        | Description                                                                     |
| ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- |
| `meta`                                                                          | [operations.GetPaymentMeta](../../models/operations/get-payment-meta.md)        | :heavy_minus_sign:                                                              | N/A                                                                             |
| `data`                                                                          | [models.PaymentResponseDto](../../models/payment-response-dto.md)               | :heavy_check_mark:                                                              | N/A                                                                             |
| `errors`                                                                        | [operations.GetPaymentErrors](../../models/operations/get-payment-errors.md)    | :heavy_check_mark:                                                              | N/A                                                                             |
| `rawData`                                                                       | [operations.GetPaymentRawData](../../models/operations/get-payment-raw-data.md) | :heavy_check_mark:                                                              | N/A                                                                             |