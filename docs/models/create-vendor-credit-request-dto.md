# CreateVendorCreditRequestDto

## Example Usage

```typescript
import { CreateVendorCreditRequestDto } from "maesn/models";

let value: CreateVendorCreditRequestDto = {
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
  currency: "Uganda Shilling",
  deliveryDate: "<value>",
  dueDate: "<value>",
  journalCode: "<value>",
  lineItems: [
    {
      id: "<id>",
      accountId: "<id>",
      accountNumber: "<value>",
      deferredEndDate: "<value>",
      deferredStartDate: "<value>",
      description:
        "however upliftingly famously favorite proper brilliant perfumed mostly",
      dimensions: [
        {
          name: "<value>",
          categoryName: "<value>",
        },
      ],
      itemId: "<id>",
      itemName: "<value>",
      quantity: 7165.76,
      taxCode: "<value>",
      taxRatePercentage: 2718.31,
      totalDiscountAmount: 9032.06,
      totalDiscountPercentage: 4280.43,
      totalGrossAmount: 8652.6,
      totalNetAmount: 4822.72,
      totalTaxAmount: 66.25,
      unitAmount: 621.12,
      unitDiscountAmount: 2697.01,
      unitDiscountPercentage: 500.78,
      unitName: "<value>",
    },
  ],
  name: "<value>",
  oneLineAddress: "<value>",
  paidDate: {},
  paymentStatus: "UNKNOWN",
  paymentDays: 4218.39,
  reference: "<value>",
  shippingDate: {},
  shippingType: "DELIVERY",
  status: "SUBMITTED",
  taxRule: "INTRACOMMUNITY_SERVICE",
  taxText: "<value>",
  totalDiscountAmount: 7077.58,
  totalDiscountPercentage: 1399.21,
  totalGrossAmount: 6078.91,
  totalNetAmount: 1673.15,
  totalTaxAmount: 6183.57,
  vendorCreditDate: "<value>",
  vendorCreditNumber: "<value>",
};
```

## Fields

| Field                                                                                                            | Type                                                                                                             | Required                                                                                                         | Description                                                                                                      |
| ---------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------- |
| `accountId`                                                                                                      | *string*                                                                                                         | :heavy_check_mark:                                                                                               | N/A                                                                                                              |
| `addresses`                                                                                                      | [models.Address](../models/address.md)[]                                                                         | :heavy_check_mark:                                                                                               | N/A                                                                                                              |
| `contactId`                                                                                                      | *string*                                                                                                         | :heavy_check_mark:                                                                                               | N/A                                                                                                              |
| `currency`                                                                                                       | *string*                                                                                                         | :heavy_check_mark:                                                                                               | N/A                                                                                                              |
| `deliveryDate`                                                                                                   | *string*                                                                                                         | :heavy_check_mark:                                                                                               | N/A                                                                                                              |
| `dueDate`                                                                                                        | *string*                                                                                                         | :heavy_check_mark:                                                                                               | N/A                                                                                                              |
| `journalCode`                                                                                                    | *string*                                                                                                         | :heavy_check_mark:                                                                                               | N/A                                                                                                              |
| `lineItems`                                                                                                      | [models.CreateVendorCreditLineItemRequestDto](../models/create-vendor-credit-line-item-request-dto.md)[]         | :heavy_check_mark:                                                                                               | N/A                                                                                                              |
| `name`                                                                                                           | *string*                                                                                                         | :heavy_check_mark:                                                                                               | N/A                                                                                                              |
| `oneLineAddress`                                                                                                 | *string*                                                                                                         | :heavy_check_mark:                                                                                               | N/A                                                                                                              |
| `paidDate`                                                                                                       | [models.CreateVendorCreditRequestDtoPaidDate](../models/create-vendor-credit-request-dto-paid-date.md)           | :heavy_check_mark:                                                                                               | N/A                                                                                                              |
| `paymentStatus`                                                                                                  | [models.CreateVendorCreditRequestDtoPaymentStatus](../models/create-vendor-credit-request-dto-payment-status.md) | :heavy_check_mark:                                                                                               | N/A                                                                                                              |
| `paymentDays`                                                                                                    | *number*                                                                                                         | :heavy_check_mark:                                                                                               | N/A                                                                                                              |
| `reference`                                                                                                      | *string*                                                                                                         | :heavy_check_mark:                                                                                               | N/A                                                                                                              |
| `shippingDate`                                                                                                   | [models.CreateVendorCreditRequestDtoShippingDate](../models/create-vendor-credit-request-dto-shipping-date.md)   | :heavy_check_mark:                                                                                               | N/A                                                                                                              |
| `shippingType`                                                                                                   | [models.CreateVendorCreditRequestDtoShippingType](../models/create-vendor-credit-request-dto-shipping-type.md)   | :heavy_check_mark:                                                                                               | N/A                                                                                                              |
| `status`                                                                                                         | [models.CreateVendorCreditRequestDtoStatus](../models/create-vendor-credit-request-dto-status.md)                | :heavy_check_mark:                                                                                               | N/A                                                                                                              |
| `taxRule`                                                                                                        | [models.CreateVendorCreditRequestDtoTaxRule](../models/create-vendor-credit-request-dto-tax-rule.md)             | :heavy_check_mark:                                                                                               | N/A                                                                                                              |
| `taxText`                                                                                                        | *string*                                                                                                         | :heavy_check_mark:                                                                                               | N/A                                                                                                              |
| `totalDiscountAmount`                                                                                            | *number*                                                                                                         | :heavy_check_mark:                                                                                               | N/A                                                                                                              |
| `totalDiscountPercentage`                                                                                        | *number*                                                                                                         | :heavy_check_mark:                                                                                               | N/A                                                                                                              |
| `totalGrossAmount`                                                                                               | *number*                                                                                                         | :heavy_check_mark:                                                                                               | N/A                                                                                                              |
| `totalNetAmount`                                                                                                 | *number*                                                                                                         | :heavy_check_mark:                                                                                               | N/A                                                                                                              |
| `totalTaxAmount`                                                                                                 | *number*                                                                                                         | :heavy_check_mark:                                                                                               | N/A                                                                                                              |
| `vendorCreditDate`                                                                                               | *string*                                                                                                         | :heavy_check_mark:                                                                                               | N/A                                                                                                              |
| `vendorCreditNumber`                                                                                             | *string*                                                                                                         | :heavy_check_mark:                                                                                               | N/A                                                                                                              |