# DeleteJournalEntryResponse

Journal entry deleted successfully

## Example Usage

```typescript
import { DeleteJournalEntryResponse } from "@maesn/typescript-sdk/models/operations";

let value: DeleteJournalEntryResponse = {
  data: {},
  errors: {},
  rawData: {},
};
```

## Fields

| Field                                                                                            | Type                                                                                             | Required                                                                                         | Description                                                                                      |
| ------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------ |
| `meta`                                                                                           | [operations.DeleteJournalEntryMeta](../../models/operations/delete-journal-entry-meta.md)        | :heavy_minus_sign:                                                                               | N/A                                                                                              |
| `data`                                                                                           | [operations.DeleteJournalEntryData](../../models/operations/delete-journal-entry-data.md)        | :heavy_check_mark:                                                                               | N/A                                                                                              |
| `errors`                                                                                         | [operations.DeleteJournalEntryErrors](../../models/operations/delete-journal-entry-errors.md)    | :heavy_check_mark:                                                                               | N/A                                                                                              |
| `rawData`                                                                                        | [operations.DeleteJournalEntryRawData](../../models/operations/delete-journal-entry-raw-data.md) | :heavy_check_mark:                                                                               | N/A                                                                                              |