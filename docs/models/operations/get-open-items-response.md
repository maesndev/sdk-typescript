# GetOpenItemsResponse

## Example Usage

```typescript
import { GetOpenItemsResponse } from "@maesn/typescript-sdk/models/operations";

let value: GetOpenItemsResponse = {
  data: [
    {
      id: "<id>",
      accountId: "<id>",
      accountName: "<value>",
      accountNumber: "<value>",
      createdDate: null,
      currency: "Namibia Dollar",
      documentNumber: "<value>",
      entries: [],
      openBalance: {
        amount: 9260.14,
        debitCreditIndicator: "CREDIT",
      },
      postingDate: "<value>",
      totalCreditAmount: 3154.92,
      totalDebitAmount: null,
      type: "INVOICE",
      updatedDate: "<value>",
    },
  ],
  errors: {},
  rawData: null,
};
```

## Fields

| Field                                                                                | Type                                                                                 | Required                                                                             | Description                                                                          |
| ------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------ |
| `meta`                                                                               | [operations.GetOpenItemsMeta](../../models/operations/get-open-items-meta.md)        | :heavy_minus_sign:                                                                   | N/A                                                                                  |
| `data`                                                                               | [models.OpenItemResponseDto](../../models/open-item-response-dto.md)[]               | :heavy_check_mark:                                                                   | N/A                                                                                  |
| `errors`                                                                             | [operations.GetOpenItemsErrors](../../models/operations/get-open-items-errors.md)    | :heavy_check_mark:                                                                   | N/A                                                                                  |
| `rawData`                                                                            | [operations.GetOpenItemsRawData](../../models/operations/get-open-items-raw-data.md) | :heavy_check_mark:                                                                   | N/A                                                                                  |