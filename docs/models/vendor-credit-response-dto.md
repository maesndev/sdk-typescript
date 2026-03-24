# VendorCreditResponseDto

## Example Usage

```typescript
import { VendorCreditResponseDto } from "maesn/models";

let value: VendorCreditResponseDto = {
  id: "<id>",
  accountId: "<id>",
  addresses: [],
  contactId: "<id>",
  createdDate: {},
  currency: "Pa'anga",
  deliveryDate: "<value>",
  dueDate: "<value>",
  fileId: "<id>",
  journalCode: "<value>",
  lineItems: [
    {
      id: "<id>",
      accountId: "<id>",
      accountNumber: "<value>",
      createdDate: "<value>",
      deferredEndDate: "<value>",
      deferredStartDate: "<value>",
      description: "foolishly pfft fooey",
      dimensions: [
        {
          name: "<value>",
          categoryName: "<value>",
        },
      ],
      itemId: "<id>",
      itemName: "<value>",
      quantity: 1855.84,
      taxCode: "<value>",
      taxRatePercentage: 2615.7,
      totalDiscountAmount: 6572,
      totalDiscountPercentage: 6452.87,
      totalGrossAmount: 3202.16,
      totalNetAmount: 7237.43,
      totalTaxAmount: 2163.58,
      unitAmount: 9075.52,
      unitDiscountAmount: 2809.3,
      unitDiscountPercentage: 1911.25,
      unitName: "<value>",
      updatedDate: "<value>",
    },
  ],
  name: "<value>",
  oneLineAddress: "<value>",
  paidDate: {},
  paymentTermId: "<id>",
  paymentStatus: "PENDING",
  paymentDays: 2221.47,
  reference: "<value>",
  shippingDate: {},
  shippingType: "SERVICE",
  status: "PARTIALLY_PAID",
  taxRule: "NET",
  taxText: "<value>",
  totalDiscountAmount: 9145.77,
  totalDiscountPercentage: 4716.18,
  totalGrossAmount: 9718.01,
  totalNetAmount: 8086.99,
  totalTaxAmount: 4476.09,
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
| `createdDate`                                                                                         | [models.VendorCreditResponseDtoCreatedDate](../models/vendor-credit-response-dto-created-date.md)     | :heavy_check_mark:                                                                                    | N/A                                                                                                   |
| `currency`                                                                                            | *string*                                                                                              | :heavy_check_mark:                                                                                    | N/A                                                                                                   |
| `deliveryDate`                                                                                        | *string*                                                                                              | :heavy_check_mark:                                                                                    | N/A                                                                                                   |
| `dueDate`                                                                                             | *string*                                                                                              | :heavy_check_mark:                                                                                    | N/A                                                                                                   |
| `fileId`                                                                                              | *string*                                                                                              | :heavy_check_mark:                                                                                    | N/A                                                                                                   |
| `journalCode`                                                                                         | *string*                                                                                              | :heavy_check_mark:                                                                                    | N/A                                                                                                   |
| `lineItems`                                                                                           | [models.VendorCreditLineItemResponseDto](../models/vendor-credit-line-item-response-dto.md)[]         | :heavy_check_mark:                                                                                    | N/A                                                                                                   |
| `name`                                                                                                | *string*                                                                                              | :heavy_check_mark:                                                                                    | N/A                                                                                                   |
| `oneLineAddress`                                                                                      | *string*                                                                                              | :heavy_check_mark:                                                                                    | N/A                                                                                                   |
| `paidDate`                                                                                            | [models.VendorCreditResponseDtoPaidDate](../models/vendor-credit-response-dto-paid-date.md)           | :heavy_check_mark:                                                                                    | N/A                                                                                                   |
| `paymentTermId`                                                                                       | *string*                                                                                              | :heavy_check_mark:                                                                                    | N/A                                                                                                   |
| `paymentStatus`                                                                                       | [models.VendorCreditResponseDtoPaymentStatus](../models/vendor-credit-response-dto-payment-status.md) | :heavy_check_mark:                                                                                    | N/A                                                                                                   |
| `paymentDays`                                                                                         | *number*                                                                                              | :heavy_check_mark:                                                                                    | N/A                                                                                                   |
| `reference`                                                                                           | *string*                                                                                              | :heavy_check_mark:                                                                                    | N/A                                                                                                   |
| `shippingDate`                                                                                        | [models.VendorCreditResponseDtoShippingDate](../models/vendor-credit-response-dto-shipping-date.md)   | :heavy_check_mark:                                                                                    | N/A                                                                                                   |
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