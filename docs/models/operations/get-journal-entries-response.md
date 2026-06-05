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
      createdDate: "<value>",
      currency: "TND",
      description:
        "knottily stunning poorly rigid near duh for wriggler knight offensively",
      documentId: "<id>",
      files: [
        "<value 1>",
        "<value 2>",
      ],
      isProvisional: true,
      journalCode: "<value>",
      journalLineItems: [
        {
          id: "<id>",
          accountCode: "<value>",
          accountId: "<id>",
          accountNumber: 6404.14,
          createdDate: null,
          currency: "CNY",
          customerId: null,
          debitCreditIndicator: "CREDIT",
          description: "till gee quaver deer",
          dimensions: [
            {
              id: "<id>",
              categoryName: "<value>",
              code: "<value>",
              name: "<value>",
            },
          ],
          documentNumber: "<value>",
          exchangeRate: 5782.76,
          supplierId: "<id>",
          taxRate: {
            id: "<id>",
            code: "<value>",
            name: "<value>",
            taxRatePercentage: "<value>",
          },
          thirdPartyCode: "<value>",
          totalGrossAmount: 6904.36,
          totalNetAmount: 1233.65,
          totalTaxAmount: 2727,
          updatedDate: "<value>",
        },
      ],
      journalType: null,
      number: "<value>",
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