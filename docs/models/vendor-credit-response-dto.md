# VendorCreditResponseDto

## Example Usage

```typescript
import { VendorCreditResponseDto } from "@maesn/typescript-sdk/models";

let value: VendorCreditResponseDto = {
  id: null,
  accountId: "<id>",
  addresses: [],
  contactId: "<id>",
  createdDate: "<value>",
  currency: null,
  deliveryDate: "<value>",
  dueDate: "<value>",
  fileId: "<id>",
  journalCode: "<value>",
  lineItems: [
    {
      id: "<id>",
      accountId: "<id>",
      accountNumber: "<value>",
      createdDate: null,
      deferredEndDate: "<value>",
      deferredStartDate: null,
      description:
        "how behind who proofread outside soulful so playfully chapel",
      dimensions: [
        {
          name: "<value>",
          categoryName: "<value>",
        },
      ],
      itemId: "<id>",
      itemName: "<value>",
      quantity: null,
      taxCode: "<value>",
      taxRatePercentage: 431.98,
      totalDiscountAmount: 9271.39,
      totalDiscountPercentage: null,
      totalGrossAmount: 4806.51,
      totalNetAmount: 8414.86,
      totalTaxAmount: 2106.05,
      unitAmount: 2688.57,
      unitDiscountAmount: 794.61,
      unitDiscountPercentage: 7940.65,
      unitName: "<value>",
      updatedDate: "<value>",
    },
  ],
  name: "<value>",
  oneLineAddress: "<value>",
  paidDate: "<value>",
  paymentReference: "<value>",
  paymentTermId: "<id>",
  paymentStatus: "CLEARED_WITH_CREDIT_NOTE",
  paymentDays: 9823.74,
  reference: "<value>",
  shippingDate: "<value>",
  shippingType: "SERVICE",
  status: "PARTIALLY_PAID",
  taxRule: "INTRACOMMUNITY_GOODS",
  taxText: "<value>",
  totalDiscountAmount: 205.22,
  totalDiscountPercentage: 3107.3,
  totalGrossAmount: 3657.5,
  totalNetAmount: 5885.96,
  totalTaxAmount: 4051.09,
  updatedDate: "<value>",
  vendorCreditDate: "<value>",
  vendorCreditNumber: "<value>",
};
```

## Fields

| Field                                                                                                 | Type                                                                                                  | Required                                                                                              | Description                                                                                           |
| ----------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------- |
| `id`                                                                                                  | *string*                                                                                              | :heavy_check_mark:                                                                                    | N/A                                                                                                   |
| `accountId`                                                                                           | *string*                                                                                              | :heavy_check_mark:                                                                                    | N/A                                                                                                   |
| `addresses`                                                                                           | [models.Address](../models/address.md)[]                                                              | :heavy_check_mark:                                                                                    | N/A                                                                                                   |
| `contactId`                                                                                           | *string*                                                                                              | :heavy_check_mark:                                                                                    | N/A                                                                                                   |
| `createdDate`                                                                                         | *string*                                                                                              | :heavy_check_mark:                                                                                    | N/A                                                                                                   |
| `currency`                                                                                            | *string*                                                                                              | :heavy_check_mark:                                                                                    | N/A                                                                                                   |
| `deliveryDate`                                                                                        | *string*                                                                                              | :heavy_check_mark:                                                                                    | N/A                                                                                                   |
| `dueDate`                                                                                             | *string*                                                                                              | :heavy_check_mark:                                                                                    | N/A                                                                                                   |
| `fileId`                                                                                              | *string*                                                                                              | :heavy_check_mark:                                                                                    | N/A                                                                                                   |
| `journalCode`                                                                                         | *string*                                                                                              | :heavy_check_mark:                                                                                    | N/A                                                                                                   |
| `lineItems`                                                                                           | [models.VendorCreditLineItemResponseDto](../models/vendor-credit-line-item-response-dto.md)[]         | :heavy_check_mark:                                                                                    | N/A                                                                                                   |
| `name`                                                                                                | *string*                                                                                              | :heavy_check_mark:                                                                                    | N/A                                                                                                   |
| `oneLineAddress`                                                                                      | *string*                                                                                              | :heavy_check_mark:                                                                                    | N/A                                                                                                   |
| `paidDate`                                                                                            | *string*                                                                                              | :heavy_check_mark:                                                                                    | N/A                                                                                                   |
| `paymentReference`                                                                                    | *string*                                                                                              | :heavy_check_mark:                                                                                    | N/A                                                                                                   |
| `paymentTermId`                                                                                       | *string*                                                                                              | :heavy_check_mark:                                                                                    | N/A                                                                                                   |
| `paymentStatus`                                                                                       | [models.VendorCreditResponseDtoPaymentStatus](../models/vendor-credit-response-dto-payment-status.md) | :heavy_check_mark:                                                                                    | N/A                                                                                                   |
| `paymentDays`                                                                                         | *number*                                                                                              | :heavy_check_mark:                                                                                    | N/A                                                                                                   |
| `reference`                                                                                           | *string*                                                                                              | :heavy_check_mark:                                                                                    | N/A                                                                                                   |
| `shippingDate`                                                                                        | *string*                                                                                              | :heavy_check_mark:                                                                                    | N/A                                                                                                   |
| `shippingType`                                                                                        | [models.VendorCreditResponseDtoShippingType](../models/vendor-credit-response-dto-shipping-type.md)   | :heavy_check_mark:                                                                                    | N/A                                                                                                   |
| `status`                                                                                              | [models.VendorCreditResponseDtoStatus](../models/vendor-credit-response-dto-status.md)                | :heavy_check_mark:                                                                                    | N/A                                                                                                   |
| `taxRule`                                                                                             | [models.VendorCreditResponseDtoTaxRule](../models/vendor-credit-response-dto-tax-rule.md)             | :heavy_check_mark:                                                                                    | N/A                                                                                                   |
| `taxText`                                                                                             | *string*                                                                                              | :heavy_check_mark:                                                                                    | N/A                                                                                                   |
| `totalDiscountAmount`                                                                                 | *number*                                                                                              | :heavy_check_mark:                                                                                    | N/A                                                                                                   |
| `totalDiscountPercentage`                                                                             | *number*                                                                                              | :heavy_check_mark:                                                                                    | N/A                                                                                                   |
| `totalGrossAmount`                                                                                    | *number*                                                                                              | :heavy_check_mark:                                                                                    | N/A                                                                                                   |
| `totalNetAmount`                                                                                      | *number*                                                                                              | :heavy_check_mark:                                                                                    | N/A                                                                                                   |
| `totalTaxAmount`                                                                                      | *number*                                                                                              | :heavy_check_mark:                                                                                    | N/A                                                                                                   |
| `updatedDate`                                                                                         | *string*                                                                                              | :heavy_check_mark:                                                                                    | N/A                                                                                                   |
| `vendorCreditDate`                                                                                    | *string*                                                                                              | :heavy_check_mark:                                                                                    | N/A                                                                                                   |
| `vendorCreditNumber`                                                                                  | *string*                                                                                              | :heavy_check_mark:                                                                                    | N/A                                                                                                   |