# CreateVendorCreditResponse

## Example Usage

```typescript
import { CreateVendorCreditResponse } from "maesn/models/operations";

let value: CreateVendorCreditResponse = {
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
    contactId: "<id>",
    createdDate: {},
    currency: "Som",
    deliveryDate: "<value>",
    dueDate: "<value>",
    fileId: "<id>",
    journalCode: "<value>",
    lineItems: [],
    name: "<value>",
    oneLineAddress: "<value>",
    paidDate: {},
    paymentTermId: "<id>",
    paymentStatus: "UNKNOWN",
    paymentDays: 2559.79,
    reference: "<value>",
    shippingDate: {},
    shippingType: "SERVICE_PERIOD",
    status: "CORRECTIVE",
    taxRule: "TAXFREE",
    taxText: "<value>",
    totalDiscountAmount: 7736.4,
    totalDiscountPercentage: 2870.91,
    totalGrossAmount: 4611.62,
    totalNetAmount: 8463.91,
    totalTaxAmount: 1547.51,
    updatedDate: "<value>",
    vendorCreditDate: "<value>",
    vendorCreditNumber: "<value>",
  },
  errors: {},
  rawData: {},
};
```

## Fields

| Field                                                                                            | Type                                                                                             | Required                                                                                         | Description                                                                                      |
| ------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------ |
| `meta`                                                                                           | [models.MetaResponse](../../models/meta-response.md)                                             | :heavy_check_mark:                                                                               | N/A                                                                                              |
| `data`                                                                                           | [models.VendorCreditResponseDto](../../models/vendor-credit-response-dto.md)                     | :heavy_check_mark:                                                                               | N/A                                                                                              |
| `errors`                                                                                         | [operations.CreateVendorCreditErrors](../../models/operations/create-vendor-credit-errors.md)    | :heavy_check_mark:                                                                               | N/A                                                                                              |
| `rawData`                                                                                        | [operations.CreateVendorCreditRawData](../../models/operations/create-vendor-credit-raw-data.md) | :heavy_check_mark:                                                                               | N/A                                                                                              |