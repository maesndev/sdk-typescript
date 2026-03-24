# CreatePaymentResponse

## Example Usage

```typescript
import { CreatePaymentResponse } from "maesn/models/operations";

let value: CreatePaymentResponse = {
  meta: {
    warnings: [
      "<value 1>",
      "<value 2>",
    ],
    pagination: {
      total: 3438.77,
      perPage: 5109.63,
      currentPage: 2626.79,
      totalPages: 3561.84,
    },
  },
  data: {
    id: "<id>",
    currency: "Belize Dollar",
    createdDate: "<value>",
    documentType: "<value>",
    exchangeRate: 8386.09,
    journalCode: "<value>",
    updatedDate: "<value>",
    paymentType: "<value>",
    paymentLines: [],
  },
  errors: {},
  rawData: {},
};
```

## Fields

| Field                                                                                 | Type                                                                                  | Required                                                                              | Description                                                                           |
| ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- |
| `meta`                                                                                | [models.MetaResponse](../../models/meta-response.md)                                  | :heavy_check_mark:                                                                    | N/A                                                                                   |
| `data`                                                                                | [models.PaymentResponseDto](../../models/payment-response-dto.md)                     | :heavy_check_mark:                                                                    | N/A                                                                                   |
| `errors`                                                                              | [operations.CreatePaymentErrors](../../models/operations/create-payment-errors.md)    | :heavy_check_mark:                                                                    | N/A                                                                                   |
| `rawData`                                                                             | [operations.CreatePaymentRawData](../../models/operations/create-payment-raw-data.md) | :heavy_check_mark:                                                                    | N/A                                                                                   |