# JournalEntriesByBatchMetaDataResponseDto

## Example Usage

```typescript
import { JournalEntriesByBatchMetaDataResponseDto } from "@maesn/typescript-sdk/models";

let value: JournalEntriesByBatchMetaDataResponseDto = {
  id: "<id>",
  accountNumberLength: 5528.21,
  chartOfAccount: "<value>",
  createdDate: "<value>",
  entries: [
    {
      id: "<id>",
      accountId: "<id>",
      accountingPeriodId: "<id>",
      createdDate: "<value>",
      currency: "XDR",
      description: "inside rear dally and once tank farm qua",
      documentId: "<id>",
      files: [],
      journalLineItems: [],
      number: "<value>",
      transactionDate: "<value>",
      updatedDate: "<value>",
    },
  ],
  fiscalYearStartDate: "<value>",
  taskId: "<id>",
};
```

## Fields

| Field                                                                       | Type                                                                        | Required                                                                    | Description                                                                 |
| --------------------------------------------------------------------------- | --------------------------------------------------------------------------- | --------------------------------------------------------------------------- | --------------------------------------------------------------------------- |
| `id`                                                                        | *string*                                                                    | :heavy_check_mark:                                                          | N/A                                                                         |
| `accountNumberLength`                                                       | *number*                                                                    | :heavy_check_mark:                                                          | N/A                                                                         |
| `chartOfAccount`                                                            | *string*                                                                    | :heavy_check_mark:                                                          | N/A                                                                         |
| `createdDate`                                                               | *string*                                                                    | :heavy_check_mark:                                                          | N/A                                                                         |
| `entries`                                                                   | [models.JournalEntryResponseDto](../models/journal-entry-response-dto.md)[] | :heavy_check_mark:                                                          | N/A                                                                         |
| `fiscalYearStartDate`                                                       | *string*                                                                    | :heavy_check_mark:                                                          | N/A                                                                         |
| `taskId`                                                                    | *string*                                                                    | :heavy_check_mark:                                                          | N/A                                                                         |