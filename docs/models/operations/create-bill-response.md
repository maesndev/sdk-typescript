# CreateBillResponse

## Example Usage

```typescript
import { CreateBillResponse } from "maesn/models/operations";

let value: CreateBillResponse = {
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
    accountId: "<id>",
    addresses: [
      {
        addressLine1: "429 Walsh Tunnel",
        addressLine2: "-",
        city: "East Melyssa",
        countryCode: "AE",
        postalCode: "39193",
        type: "SELLING",
      },
    ],
    billDate: "<value>",
    billNumber: "<value>",
    contactId: "<id>",
    createdDate: {},
    currency: "Lek",
    deliveryDate: "<value>",
    dueDate: "<value>",
    fileId: "<id>",
    journalCode: "<value>",
    lineItems: [],
    name: "<value>",
    oneLineAddress: "<value>",
    paidDate: {},
    paymentTermCode: "<value>",
    paymentStatus: "CANCELED",
    paymentDays: 8483.35,
    reference: "<value>",
    shippingDate: {},
    shippingType: "DELIVERY_PERIOD",
    status: "DOCUMENT_CREATED",
    taxRule: "OSS_SERVICES",
    taxText: "<value>",
    totalDiscountAmount: 3581.38,
    totalDiscountPercentage: 7267.68,
    totalGrossAmount: 955.76,
    totalNetAmount: 2328.09,
    totalTaxAmount: 2090.04,
    updatedDate: "<value>",
  },
  errors: {},
  rawData: {},
};
```

## Fields

| Field                                                                           | Type                                                                            | Required                                                                        | Description                                                                     |
| ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- |
| `meta`                                                                          | [models.MetaResponse](../../models/meta-response.md)                            | :heavy_check_mark:                                                              | N/A                                                                             |
| `data`                                                                          | [models.BillResponseDto](../../models/bill-response-dto.md)                     | :heavy_check_mark:                                                              | N/A                                                                             |
| `errors`                                                                        | [operations.CreateBillErrors](../../models/operations/create-bill-errors.md)    | :heavy_check_mark:                                                              | N/A                                                                             |
| `rawData`                                                                       | [operations.CreateBillRawData](../../models/operations/create-bill-raw-data.md) | :heavy_check_mark:                                                              | N/A                                                                             |