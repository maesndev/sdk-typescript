# GetOpenItemsResponse

## Example Usage

```typescript
import { GetOpenItemsResponse } from "maesn/models/operations";

let value: GetOpenItemsResponse = {
  meta: {
    warnings: [
      "<value 1>",
      "<value 2>",
    ],
    pagination: {
      total: 3438.77,
      perPage: 5109.63,
      currentPage: 2626.79,
      totalPages: 3561.84,
    },
  },
  data: [
    {
      id: "<id>",
      accountId: "<id>",
      accountName: "<value>",
      accountNumber: "<value>",
      createdDate: "<value>",
      currency: "Burundi Franc",
      documentNumber: "<value>",
      entries: [
        {
          amount: 5250.91,
          currency: "Balboa",
          debitCreditIndicator: "DEBIT",
          description: "variable swear wherever per ack jazz during with until",
          dueDate: "<value>",
          postingDate: "<value>",
        },
      ],
      openBalance: {
        amount: 7475.92,
        debitCreditIndicator: "DEBIT",
      },
      postingDate: "<value>",
      totalCreditAmount: 2700.29,
      totalDebitAmount: 485.03,
      type: "INVOICE",
      updatedDate: "<value>",
    },
  ],
  errors: {},
  rawData: {},
};
```

## Fields

| Field                                                                                | Type                                                                                 | Required                                                                             | Description                                                                          |
| ------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------ |
| `meta`                                                                               | [models.MetaResponse](../../models/meta-response.md)                                 | :heavy_check_mark:                                                                   | N/A                                                                                  |
| `data`                                                                               | [models.OpenItemResponseDto](../../models/open-item-response-dto.md)[]               | :heavy_check_mark:                                                                   | N/A                                                                                  |
| `errors`                                                                             | [operations.GetOpenItemsErrors](../../models/operations/get-open-items-errors.md)    | :heavy_check_mark:                                                                   | N/A                                                                                  |
| `rawData`                                                                            | [operations.GetOpenItemsRawData](../../models/operations/get-open-items-raw-data.md) | :heavy_check_mark:                                                                   | N/A                                                                                  |