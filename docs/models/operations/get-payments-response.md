# GetPaymentsResponse

## Example Usage

```typescript
import { GetPaymentsResponse } from "maesn/models/operations";

let value: GetPaymentsResponse = {
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
  data: [
    {
      id: "<id>",
      currency: "Cuban Peso",
      createdDate: "<value>",
      documentType: "<value>",
      exchangeRate: 3678.96,
      journalCode: "<value>",
      updatedDate: "<value>",
      paymentType: "<value>",
      paymentLines: [],
    },
  ],
  errors: {},
  rawData: {},
};
```

## Fields

| Field                                                                             | Type                                                                              | Required                                                                          | Description                                                                       |
| --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- |
| `meta`                                                                            | [models.MetaResponse](../../models/meta-response.md)                              | :heavy_check_mark:                                                                | N/A                                                                               |
| `data`                                                                            | [models.PaymentResponseDto](../../models/payment-response-dto.md)[]               | :heavy_check_mark:                                                                | N/A                                                                               |
| `errors`                                                                          | [operations.GetPaymentsErrors](../../models/operations/get-payments-errors.md)    | :heavy_check_mark:                                                                | N/A                                                                               |
| `rawData`                                                                         | [operations.GetPaymentsRawData](../../models/operations/get-payments-raw-data.md) | :heavy_check_mark:                                                                | N/A                                                                               |