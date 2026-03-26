# CreateJournalEntriesByBatchMetaDataDto

## Example Usage

```typescript
import { CreateJournalEntriesByBatchMetaDataDto } from "@maesn/typescript-sdk/models";

let value: CreateJournalEntriesByBatchMetaDataDto = {
  accountNumberLength: 9051.58,
  chartOfAccount: "SKR14",
  entries: [
    {},
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