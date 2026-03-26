# CreateJournalEntriesRequest

## Example Usage

```typescript
import { CreateJournalEntriesRequest } from "@maesn/typescript-sdk/models/operations";

let value: CreateJournalEntriesRequest = {
  body: {
    accountNumberLength: 5521.98,
    chartOfAccount: "SKR14",
    entries: [],
    fiscalYearStartDate: "<value>",
  },
};
```

## Fields

| Field                                                                                                          | Type                                                                                                           | Required                                                                                                       | Description                                                                                                    |
| -------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------- |
| `companyId`                                                                                                    | *string*                                                                                                       | :heavy_minus_sign:                                                                                             | N/A                                                                                                            |
| `body`                                                                                                         | [models.CreateJournalEntriesByBatchMetaDataDto](../../models/create-journal-entries-by-batch-meta-data-dto.md) | :heavy_check_mark:                                                                                             | N/A                                                                                                            |