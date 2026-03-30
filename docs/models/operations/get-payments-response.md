# GetPaymentsResponse

List of payments for the authenticated end user's connected target system

## Example Usage

```typescript
import { GetPaymentsResponse } from "@maesn/typescript-sdk/models/operations";

let value: GetPaymentsResponse = {
  data: [
    {
      id: "<id>",
      currency: "Guinea Franc",
      createdDate: "<value>",
      documentType: "INVOICE",
      exchangeRate: 7484.63,
      journalCode: null,
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
| `meta`                                                                            | [operations.GetPaymentsMeta](../../models/operations/get-payments-meta.md)        | :heavy_minus_sign:                                                                | N/A                                                                               |
| `data`                                                                            | [models.PaymentResponseDto](../../models/payment-response-dto.md)[]               | :heavy_check_mark:                                                                | N/A                                                                               |
| `errors`                                                                          | [operations.GetPaymentsErrors](../../models/operations/get-payments-errors.md)    | :heavy_check_mark:                                                                | N/A                                                                               |
| `rawData`                                                                         | [operations.GetPaymentsRawData](../../models/operations/get-payments-raw-data.md) | :heavy_check_mark:                                                                | N/A                                                                               |