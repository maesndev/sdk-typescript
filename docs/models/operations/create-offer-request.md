# CreateOfferRequest

## Example Usage

```typescript
import { CreateOfferRequest } from "maesn/models/operations";

let value: CreateOfferRequest = {
  body: {
    addresses: [],
    contactId: "<id>",
    currency: "Barbados Dollar",
    lineItems: [
      {
        accountCode: "<value>",
        accountId: "<id>",
        description:
          "collaborate inasmuch maroon fearless whoa fortunately pushy nervous",
        itemId: "<id>",
        name: "<value>",
        quantity: 4019.85,
        taxCode: "<value>",
        taxRatePercentage: 8523.99,
        taxType: "<value>",
        type: "VALUE",
        totalDiscountAmount: 2373.54,
        totalDiscountPercentage: 243.82,
        totalGrossAmount: 8759.59,
        totalNetAmount: 1178.65,
        totalTaxAmount: 4228.69,
        unitAmount: 361.83,
        unitDiscountAmount: 4878.94,
        unitDiscountPercentage: 5160.82,
        unitName: "<value>",
      },
    ],
    name: "<value>",
    offerDate: "<value>",
    offerNumber: "<value>",
    oneLineAddress: "<value>",
    reference: "<value>",
    status: "VOIDED",
    taxText: "<value>",
    totalDiscountAmount: 9712.98,
    totalDiscountPercentage: 6587.3,
    totalGrossAmount: 943.9,
    totalNetAmount: 3467.32,
    totalTaxAmount: 1807.97,
  },
};
```

## Fields

| Field                                                                    | Type                                                                     | Required                                                                 | Description                                                              |
| ------------------------------------------------------------------------ | ------------------------------------------------------------------------ | ------------------------------------------------------------------------ | ------------------------------------------------------------------------ |
| `environmentName`                                                        | *string*                                                                 | :heavy_minus_sign:                                                       | N/A                                                                      |
| `companyId`                                                              | *string*                                                                 | :heavy_minus_sign:                                                       | N/A                                                                      |
| `body`                                                                   | [models.CreateOfferRequestDto](../../models/create-offer-request-dto.md) | :heavy_check_mark:                                                       | N/A                                                                      |