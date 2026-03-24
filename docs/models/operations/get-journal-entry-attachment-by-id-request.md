# GetJournalEntryAttachmentByIdRequest

## Example Usage

```typescript
import { GetJournalEntryAttachmentByIdRequest } from "maesn/models/operations";

let value: GetJournalEntryAttachmentByIdRequest = {
  journalEntryId: "<id>",
  attachmentId: "<id>",
};
```

## Fields

| Field              | Type               | Required           | Description        |
| ------------------ | ------------------ | ------------------ | ------------------ |
| `journalEntryId`   | *string*           | :heavy_check_mark: | N/A                |
| `attachmentId`     | *string*           | :heavy_check_mark: | N/A                |
| `environmentName`  | *string*           | :heavy_minus_sign: | N/A                |
| `companyId`        | *string*           | :heavy_minus_sign: | N/A                |
| `xApiKey`          | *string*           | :heavy_minus_sign: | API key            |
| `xAccountKey`      | *string*           | :heavy_minus_sign: | Account key        |