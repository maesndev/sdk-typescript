# CreateVendorCreditResponse

## Example Usage

```typescript
import { CreateVendorCreditResponse } from "@maesn/typescript-sdk/models/operations";

let value: CreateVendorCreditResponse = {
  data: {
    id: "<id>",
    accountId: "<id>",
    addresses: [
      {},
    ],
    contactId: "<id>",
    createdDate: "<value>",
    currency: "Bulgarian Lev",
    deliveryDate: "<value>",
    dueDate: "<value>",
    fileId: "<id>",
    journalCode: "<value>",
    lineItems: [],
    name: null,
    oneLineAddress: "<value>",
    paidDate: "<value>",
    paymentTermId: "<id>",
    paymentStatus: "DEBITED",
    paymentDays: 9755.3,
    reference: "<value>",
    shippingDate: "<value>",
    shippingType: "DELIVERY",
    status: "PARTIALLY_OVERDUE",
    taxRule: "SMALL_BUSINESS_EXEMPTION",
    taxText: "<value>",
    totalDiscountAmount: 5408.68,
    totalDiscountPercentage: 5825.03,
    totalGrossAmount: 4147.12,
    totalNetAmount: 6941.2,
    totalTaxAmount: 7325.33,
    updatedDate: null,
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
| `meta`                                                                                           | [operations.CreateVendorCreditMeta](../../models/operations/create-vendor-credit-meta.md)        | :heavy_minus_sign:                                                                               | N/A                                                                                              |
| `data`                                                                                           | [models.VendorCreditResponseDto](../../models/vendor-credit-response-dto.md)                     | :heavy_check_mark:                                                                               | N/A                                                                                              |
| `errors`                                                                                         | [operations.CreateVendorCreditErrors](../../models/operations/create-vendor-credit-errors.md)    | :heavy_check_mark:                                                                               | N/A                                                                                              |
| `rawData`                                                                                        | [operations.CreateVendorCreditRawData](../../models/operations/create-vendor-credit-raw-data.md) | :heavy_check_mark:                                                                               | N/A                                                                                              |