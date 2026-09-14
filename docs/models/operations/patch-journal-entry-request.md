# PatchJournalEntryRequest

## Example Usage

```typescript
import { PatchJournalEntryRequest } from "@maesn/typescript-sdk/models/operations";

let value: PatchJournalEntryRequest = {
  journalEntryId: "<id>",
  body: {},
};
```

## Fields

| Field                                                                                                  | Type                                                                                                   | Required                                                                                               | Description                                                                                            |
| ------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------ |
| `journalEntryId`                                                                                       | *string*                                                                                               | :heavy_check_mark:                                                                                     | N/A                                                                                                    |
| `companyId`                                                                                            | *string*                                                                                               | :heavy_minus_sign:                                                                                     | ID of the company (required for multi-company target systems)                                          |
| `apiKey`                                                                                               | *string*                                                                                               | :heavy_minus_sign:                                                                                     | API key                                                                                                |
| `accountKey`                                                                                           | *string*                                                                                               | :heavy_minus_sign:                                                                                     | Account key                                                                                            |
| `body`                                                                                                 | [operations.PatchJournalEntryRequestBody](../../models/operations/patch-journal-entry-request-body.md) | :heavy_check_mark:                                                                                     | N/A                                                                                                    |