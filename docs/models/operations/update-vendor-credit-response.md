# UpdateVendorCreditResponse

Vendor credit updated successfully

## Example Usage

```typescript
import { UpdateVendorCreditResponse } from "@maesn/typescript-sdk/models/operations";

let value: UpdateVendorCreditResponse = {
  data: {
    id: "<id>",
    accountId: null,
    addresses: null,
    billDate: "<value>",
    billNumber: "<value>",
    contactId: "<id>",
    createdDate: "<value>",
    currency: "Forint",
    deliveryDate: "<value>",
    dueDate: null,
    fileId: "<id>",
    journalCode: "<value>",
    lineItems: [
      {
        id: "<id>",
        accountId: null,
        accountNumber: "<value>",
        createdDate: "<value>",
        deferredEndDate: "<value>",
        deferredStartDate: "<value>",
        description: "oof dish ouch rotten mortar giant",
        dimensions: [],
        itemId: "<id>",
        itemName: "<value>",
        quantity: 8319.09,
        taxCode: "<value>",
        taxRatePercentage: 4598.12,
        totalDiscountAmount: 7548.91,
        totalDiscountPercentage: 5308.45,
        totalGrossAmount: 5588.18,
        totalNetAmount: 1273.27,
        totalTaxAmount: 7450.14,
        unitAmount: 4776.62,
        unitDiscountAmount: 6000.9,
        unitDiscountPercentage: 4093.91,
        unitName: "<value>",
        updatedDate: "<value>",
      },
    ],
    name: "<value>",
    oneLineAddress: "<value>",
    paidDate: null,
    paymentTermCode: "<value>",
    paymentStatus: "NO_OPEN_ITEM",
    paymentDays: 9445.21,
    reference: "<value>",
    shippingDate: "<value>",
    shippingType: "DELIVERY_PERIOD",
    status: "PARTIALLY_PAID",
    taxRule: "NON_DOMESTIC_SERVICE",
    taxText: "<value>",
    totalDiscountAmount: 7147.68,
    totalDiscountPercentage: 9868.83,
    totalGrossAmount: 4883.34,
    totalNetAmount: 4247.21,
    totalTaxAmount: 7337.62,
    updatedDate: "<value>",
  },
  errors: {},
  rawData: null,
};
```

## Fields

| Field                                                                                            | Type                                                                                             | Required                                                                                         | Description                                                                                      |
| ------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------ |
| `meta`                                                                                           | [operations.UpdateVendorCreditMeta](../../models/operations/update-vendor-credit-meta.md)        | :heavy_minus_sign:                                                                               | N/A                                                                                              |
| `data`                                                                                           | [models.BillResponseDto](../../models/bill-response-dto.md)                                      | :heavy_check_mark:                                                                               | N/A                                                                                              |
| `errors`                                                                                         | [operations.UpdateVendorCreditErrors](../../models/operations/update-vendor-credit-errors.md)    | :heavy_check_mark:                                                                               | N/A                                                                                              |
| `rawData`                                                                                        | [operations.UpdateVendorCreditRawData](../../models/operations/update-vendor-credit-raw-data.md) | :heavy_check_mark:                                                                               | N/A                                                                                              |