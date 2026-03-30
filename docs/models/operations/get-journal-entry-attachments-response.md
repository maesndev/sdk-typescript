# GetJournalEntryAttachmentsResponse

List of attachments for the journal entry matching the provided ID

## Example Usage

```typescript
import { GetJournalEntryAttachmentsResponse } from "@maesn/typescript-sdk/models/operations";

let value: GetJournalEntryAttachmentsResponse = {
  data: [],
  errors: {},
  rawData: {},
};
```

## Fields

| Field                                                                                                             | Type                                                                                                              | Required                                                                                                          | Description                                                                                                       |
| ----------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------- |
| `meta`                                                                                                            | [operations.GetJournalEntryAttachmentsMeta](../../models/operations/get-journal-entry-attachments-meta.md)        | :heavy_minus_sign:                                                                                                | N/A                                                                                                               |
| `data`                                                                                                            | [models.JournalEntryResponseDto](../../models/journal-entry-response-dto.md)[]                                    | :heavy_check_mark:                                                                                                | N/A                                                                                                               |
| `errors`                                                                                                          | [operations.GetJournalEntryAttachmentsErrors](../../models/operations/get-journal-entry-attachments-errors.md)    | :heavy_check_mark:                                                                                                | N/A                                                                                                               |
| `rawData`                                                                                                         | [operations.GetJournalEntryAttachmentsRawData](../../models/operations/get-journal-entry-attachments-raw-data.md) | :heavy_check_mark:                                                                                                | N/A                                                                                                               |