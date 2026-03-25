# CreateBillRequest

## Example Usage

```typescript
import { CreateBillRequest } from "maesn/models/operations";

let value: CreateBillRequest = {
  body: {
    accountId: "<id>",
    addresses: [],
    billDate: "<value>",
    billNumber: "<value>",
    contactId: "<id>",
    currency: "Leone",
    deliveryDate: "<value>",
    dueDate: "<value>",
    fileId: "<id>",
    journalCode: "<value>",
    lineItems: [
      {
        id: "<id>",
        accountId: "<id>",
        accountNumber: "<value>",
        deferredEndDate: "<value>",
        deferredStartDate: "<value>",
        description:
          "whose sedately zowie soon yowza solemnly step-mother painfully phooey",
        dimensions: [],
        itemId: "<id>",
        itemName: "<value>",
        quantity: 5519.84,
        taxCode: "<value>",
        taxRatePercentage: 4194.04,
        totalDiscountAmount: 2979.82,
        totalDiscountPercentage: 6926.8,
        totalGrossAmount: 9233.58,
        totalNetAmount: 1233.01,
        totalTaxAmount: 8119.37,
        unitAmount: 4907.85,
        unitDiscountAmount: 1684.91,
        unitDiscountPercentage: 9320.51,
        unitName: "<value>",
      },
    ],
    name: "<value>",
    oneLineAddress: "<value>",
    paidDate: {},
    paymentTermCode: "<value>",
    paymentStatus: "UNKNOWN",
    paymentDays: 3012.79,
    reference: "<value>",
    shippingDate: {},
    shippingType: "SERVICE_PERIOD",
    status: "DRAFT",
    taxRule: "OSS_ELECTRONIC_SERVICES",
    taxText: "<value>",
    totalDiscountAmount: 151.45,
    totalDiscountPercentage: 574.12,
    totalGrossAmount: 7985.55,
    totalNetAmount: 4774.8,
    totalTaxAmount: 8066.72,
  },
};
```

## Fields

| Field                                                                  | Type                                                                   | Required                                                               | Description                                                            |
| ---------------------------------------------------------------------- | ---------------------------------------------------------------------- | ---------------------------------------------------------------------- | ---------------------------------------------------------------------- |
| `environmentName`                                                      | *string*                                                               | :heavy_minus_sign:                                                     | N/A                                                                    |
| `companyId`                                                            | *string*                                                               | :heavy_minus_sign:                                                     | N/A                                                                    |
| `body`                                                                 | [models.CreateBillRequestDto](../../models/create-bill-request-dto.md) | :heavy_check_mark:                                                     | N/A                                                                    |