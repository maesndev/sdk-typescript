# GetJournalEntryResponse

## Example Usage

```typescript
import { GetJournalEntryResponse } from "maesn/models/operations";

let value: GetJournalEntryResponse = {
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
      accountingPeriodId: "<id>",
      createdDate: "<value>",
      currency: "CHF",
      debitCreditIndicator: "DEBIT",
      deliveryDate: "<value>",
      description: "revoke mutate austere",
      documentId: "<id>",
      dueDate: "<value>",
      exchangeRate: "<value>",
      files: [],
      isProvisional: true,
      journalCode: "<value>",
      journalLineItems: [
        "<value 1>",
        "<value 2>",
      ],
      journalType: "<value>",
      number: "<value>",
      taxAssignmentDate: "<value>",
      transactionDate: "<value>",
      updatedDate: "<value>",
    },
  ],
  errors: {},
  rawData: {},
};
```

## Fields

| Field                                                                                      | Type                                                                                       | Required                                                                                   | Description                                                                                |
| ------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------ |
| `meta`                                                                                     | [models.MetaResponse](../../models/meta-response.md)                                       | :heavy_check_mark:                                                                         | N/A                                                                                        |
| `data`                                                                                     | [models.JournalEntryResponseDto](../../models/journal-entry-response-dto.md)[]             | :heavy_check_mark:                                                                         | N/A                                                                                        |
| `errors`                                                                                   | [operations.GetJournalEntryErrors](../../models/operations/get-journal-entry-errors.md)    | :heavy_check_mark:                                                                         | N/A                                                                                        |
| `rawData`                                                                                  | [operations.GetJournalEntryRawData](../../models/operations/get-journal-entry-raw-data.md) | :heavy_check_mark:                                                                         | N/A                                                                                        |