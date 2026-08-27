# UpdateJournalEntryRequest

## Example Usage

```typescript
import { UpdateJournalEntryRequest } from "@maesn/typescript-sdk/models/operations";

let value: UpdateJournalEntryRequest = {
  journalEntryId: "<id>",
  body: {},
};
```

## Fields

| Field                                                                                                    | Type                                                                                                     | Required                                                                                                 | Description                                                                                              |
| -------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------- |
| `journalEntryId`                                                                                         | *string*                                                                                                 | :heavy_check_mark:                                                                                       | N/A                                                                                                      |
| `companyId`                                                                                              | *string*                                                                                                 | :heavy_minus_sign:                                                                                       | ID of the company (required for multi-company target systems)                                            |
| `apiKey`                                                                                                 | *string*                                                                                                 | :heavy_minus_sign:                                                                                       | API key                                                                                                  |
| `accountKey`                                                                                             | *string*                                                                                                 | :heavy_minus_sign:                                                                                       | Account key                                                                                              |
| `body`                                                                                                   | [operations.UpdateJournalEntryRequestBody](../../models/operations/update-journal-entry-request-body.md) | :heavy_check_mark:                                                                                       | N/A                                                                                                      |