# CreateCreditNoteResponse

Credit note created successfully

## Example Usage

```typescript
import { CreateCreditNoteResponse } from "@maesn/typescript-sdk/models/operations";

let value: CreateCreditNoteResponse = {
  data: {
    id: "<id>",
    addresses: [
      {},
    ],
    contactId: "<id>",
    createdDate: "<value>",
    creditNoteDate: "<value>",
    creditNoteLines: [
      {
        id: "<id>",
        createdDate: "<value>",
        description: "replacement swift mmm",
        itemId: "<id>",
        itemName: "<value>",
        quantity: 7964.31,
        taxCode: "<value>",
        taxRatePercentage: 2289.85,
        totalDiscountAmount: 2224.65,
        totalDiscountPercentage: 8636.87,
        totalGrossAmount: null,
        totalNetAmount: 8637.84,
        totalTaxAmount: 2022.47,
        type: "MATERIAL",
        unitAmount: 7633.55,
        unitDiscountAmount: null,
        unitDiscountPercentage: 5313.04,
        unitName: "<value>",
        updatedDate: null,
      },
    ],
    creditNoteNumber: "<value>",
    currency: "Burundi Franc",
    paymentStatus: "PENDING",
    paymentTermId: "<id>",
    reference: "<value>",
    status: "VOIDED",
    taxRule: "GROSS",
    totalDiscountAmount: 1916.47,
    totalDiscountPercentage: 732.08,
    totalGrossAmount: 8273.2,
    totalNetAmount: 8820.33,
    totalTaxAmount: 360.27,
    updatedDate: "<value>",
  },
  errors: null,
  rawData: {},
};
```

## Fields

| Field                                                                                        | Type                                                                                         | Required                                                                                     | Description                                                                                  |
| -------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------- |
| `meta`                                                                                       | [operations.CreateCreditNoteMeta](../../models/operations/create-credit-note-meta.md)        | :heavy_minus_sign:                                                                           | N/A                                                                                          |
| `data`                                                                                       | [models.CreditNoteResponseDto](../../models/credit-note-response-dto.md)                     | :heavy_check_mark:                                                                           | N/A                                                                                          |
| `errors`                                                                                     | [operations.CreateCreditNoteErrors](../../models/operations/create-credit-note-errors.md)    | :heavy_check_mark:                                                                           | N/A                                                                                          |
| `rawData`                                                                                    | [operations.CreateCreditNoteRawData](../../models/operations/create-credit-note-raw-data.md) | :heavy_check_mark:                                                                           | N/A                                                                                          |