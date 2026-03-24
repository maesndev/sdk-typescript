# JournalEntriesByBatchMetaDataResponseDto

## Example Usage

```typescript
import { JournalEntriesByBatchMetaDataResponseDto } from "maesn/models";

let value: JournalEntriesByBatchMetaDataResponseDto = {
  id: "<id>",
  accountNumberLength: 1245.22,
  chartOfAccount: "<value>",
  createdDate: "<value>",
  entries: [],
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