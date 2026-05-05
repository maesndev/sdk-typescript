# CreateVendorCreditResponse

Vendor credit created successfully

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
    paymentReference: "<value>",
    paymentTermId: "<id>",
    paymentStatus: "PENDING",
    paymentDays: 2391.09,
    reference: "<value>",
    shippingDate: "<value>",
    shippingType: "DELIVERY",
    status: "SUBMITTED",
    taxRule: "INTRACOMMUNITY_GOODS",
    taxText: "<value>",
    totalDiscountAmount: 4543.97,
    totalDiscountPercentage: 1043.34,
    totalGrossAmount: 6999.54,
    totalNetAmount: 1981.27,
    totalTaxAmount: 734.34,
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
| `meta`                                                                                           | [operations.CreateVendorCreditMeta](../../models/operations/create-vendor-credit-meta.md)        | :heavy_minus_sign:                                                                               | N/A                                                                                              |
| `data`                                                                                           | [models.VendorCreditResponseDto](../../models/vendor-credit-response-dto.md)                     | :heavy_check_mark:                                                                               | N/A                                                                                              |
| `errors`                                                                                         | [operations.CreateVendorCreditErrors](../../models/operations/create-vendor-credit-errors.md)    | :heavy_check_mark:                                                                               | N/A                                                                                              |
| `rawData`                                                                                        | [operations.CreateVendorCreditRawData](../../models/operations/create-vendor-credit-raw-data.md) | :heavy_check_mark:                                                                               | N/A                                                                                              |