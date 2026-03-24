# UpdateVendorCreditRequest

## Example Usage

```typescript
import { UpdateVendorCreditRequest } from "maesn/models/operations";

let value: UpdateVendorCreditRequest = {
  vendorCreditId: "<id>",
  body: {
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
    currency: "UAE Dirham",
    deliveryDate: "<value>",
    dueDate: "<value>",
    journalCode: "<value>",
    lineItems: [],
    name: "<value>",
    oneLineAddress: "<value>",
    paidDate: {},
    paymentStatus: "PAID",
    paymentDays: 6582.46,
    reference: "<value>",
    shippingDate: {},
    shippingType: "DELIVERY_PERIOD",
    status: "DOCUMENT_CREATED",
    taxRule: "NET",
    taxText: "<value>",
    totalDiscountAmount: 107.12,
    totalDiscountPercentage: 6996.21,
    totalGrossAmount: 3198.29,
    totalNetAmount: 733.02,
    totalTaxAmount: 7693.93,
    vendorCreditDate: "<value>",
    vendorCreditNumber: "<value>",
  },
};
```

## Fields

| Field                                                                                   | Type                                                                                    | Required                                                                                | Description                                                                             |
| --------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------- |
| `vendorCreditId`                                                                        | *string*                                                                                | :heavy_check_mark:                                                                      | N/A                                                                                     |
| `environmentName`                                                                       | *string*                                                                                | :heavy_minus_sign:                                                                      | N/A                                                                                     |
| `companyId`                                                                             | *string*                                                                                | :heavy_minus_sign:                                                                      | N/A                                                                                     |
| `xApiKey`                                                                               | *string*                                                                                | :heavy_minus_sign:                                                                      | API key                                                                                 |
| `xAccountKey`                                                                           | *string*                                                                                | :heavy_minus_sign:                                                                      | Account key                                                                             |
| `body`                                                                                  | [models.CreateVendorCreditRequestDto](../../models/create-vendor-credit-request-dto.md) | :heavy_check_mark:                                                                      | N/A                                                                                     |