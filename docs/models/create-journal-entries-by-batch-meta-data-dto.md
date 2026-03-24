# CreateJournalEntriesByBatchMetaDataDto

## Example Usage

```typescript
import { CreateJournalEntriesByBatchMetaDataDto } from "maesn/models";

let value: CreateJournalEntriesByBatchMetaDataDto = {
  accountNumberLength: 9051.58,
  chartOfAccount: "SKR14",
  entries: [
    {
      accountId: "<id>",
      accountingPeriodId: "<id>",
      currency: "BGN",
      debitCreditIndicator: "DEBIT",
      deliveryDate: "<value>",
      description: "parsnip decriminalize including blah since catalyze openly",
      documentId: "<id>",
      dueDate: "<value>",
      exchangeRate: "<value>",
      isProvisional: false,
      journalCode: "<value>",
      journalLineItems: [
        {
          accountCode: "<value>",
          accountId: "<id>",
          accountNumber: 5924.3,
          currency: "SZL",
          customerId: "<id>",
          debitCreditIndicator: "CREDIT",
          description: "misguided worth since provided average waltz",
          dimensions: [
            "<value 1>",
          ],
          discountAmount: 6082.9,
          documentNumber: "<value>",
          exchangeRate: "<value>",
          supplierId: "<id>",
          taxRate: {
            id: "<id>",
            code: "<value>",
            name: "<value>",
            taxRatePercentage: "<value>",
          },
          thirdPartyCode: "<value>",
          totalGrossAmount: 2944.04,
          totalNetAmount: 6946.54,
          totalTaxAmount: 9131.3,
        },
      ],
      journalType: "<value>",
      number: "<value>",
      taxAssignmentDate: "<value>",
      transactionDate: "<value>",
    },
  ],
  fiscalYearStartDate: "<value>",
};
```

## Fields

| Field                                                                                                                                      | Type                                                                                                                                       | Required                                                                                                                                   | Description                                                                                                                                |
| ------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------ |
| `accountNumberLength`                                                                                                                      | *number*                                                                                                                                   | :heavy_check_mark:                                                                                                                         | N/A                                                                                                                                        |
| `chartOfAccount`                                                                                                                           | [models.CreateJournalEntriesByBatchMetaDataDtoChartOfAccount](../models/create-journal-entries-by-batch-meta-data-dto-chart-of-account.md) | :heavy_check_mark:                                                                                                                         | N/A                                                                                                                                        |
| `entries`                                                                                                                                  | [models.CreateJournalEntryRequestDto](../models/create-journal-entry-request-dto.md)[]                                                     | :heavy_check_mark:                                                                                                                         | N/A                                                                                                                                        |
| `fiscalYearStartDate`                                                                                                                      | *string*                                                                                                                                   | :heavy_check_mark:                                                                                                                         | N/A                                                                                                                                        |