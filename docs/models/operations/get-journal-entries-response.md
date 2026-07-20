# GetJournalEntriesResponse

List of journal entries for the authenticated end user's connected target system

## Example Usage

```typescript
import { GetJournalEntriesResponse } from "@maesn/typescript-sdk/models/operations";

let value: GetJournalEntriesResponse = {
  data: [
    {
      id: "<id>",
      accountId: "<id>",
      accountingPeriodId: null,
      accountingReason: "CALCULATION",
      createdDate: "<value>",
      currency: "VEB",
      description:
        "mutate austere under close helpless enthusiastically humor total",
      documentId: null,
      files: [
        "<value 1>",
        "<value 2>",
        "<value 3>",
      ],
      isProvisional: false,
      isReversal: null,
      journalCode: "<value>",
      journalLineItems: [
        {
          id: "<id>",
          accountCode: "<value>",
          accountId: "<id>",
          accountNumber: 9591.91,
          createdDate: "<value>",
          currency: "KYD",
          customerId: "<id>",
          debitCreditIndicator: "CREDIT",
          description: "after to content scrap aw",
          dimensions: null,
          documentId: "<id>",
          documentNumber: "<value>",
          exchangeRate: 9682.62,
          supplierId: "<id>",
          taxRate: {
            id: "<id>",
            code: "<value>",
            name: "<value>",
            taxRatePercentage: "<value>",
          },
          thirdPartyCode: "<value>",
          totalGrossAmount: 5036,
          totalNetAmount: 9416.06,
          totalTaxAmount: 8710.22,
          updatedDate: "<value>",
        },
      ],
      journalType: "<value>",
      number: "<value>",
      recordType: "STANDARD",
      transactionDate: "<value>",
      updatedDate: "<value>",
    },
  ],
  errors: {},
  rawData: {},
};
```

## Fields

| Field                                                                                          | Type                                                                                           | Required                                                                                       | Description                                                                                    |
| ---------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------- |
| `meta`                                                                                         | [operations.GetJournalEntriesMeta](../../models/operations/get-journal-entries-meta.md)        | :heavy_minus_sign:                                                                             | N/A                                                                                            |
| `data`                                                                                         | [models.JournalEntryResponseDto](../../models/journal-entry-response-dto.md)[]                 | :heavy_check_mark:                                                                             | N/A                                                                                            |
| `errors`                                                                                       | [operations.GetJournalEntriesErrors](../../models/operations/get-journal-entries-errors.md)    | :heavy_check_mark:                                                                             | N/A                                                                                            |
| `rawData`                                                                                      | [operations.GetJournalEntriesRawData](../../models/operations/get-journal-entries-raw-data.md) | :heavy_check_mark:                                                                             | N/A                                                                                            |