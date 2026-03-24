# CreateJournalEntryRequest

## Example Usage

```typescript
import { CreateJournalEntryRequest } from "maesn/models/operations";

let value: CreateJournalEntryRequest = {
  body: {},
};
```

## Fields

| Field                                                                                                    | Type                                                                                                     | Required                                                                                                 | Description                                                                                              |
| -------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------- |
| `environmentName`                                                                                        | *string*                                                                                                 | :heavy_minus_sign:                                                                                       | N/A                                                                                                      |
| `companyId`                                                                                              | *string*                                                                                                 | :heavy_minus_sign:                                                                                       | N/A                                                                                                      |
| `xApiKey`                                                                                                | *string*                                                                                                 | :heavy_minus_sign:                                                                                       | API key                                                                                                  |
| `xAccountKey`                                                                                            | *string*                                                                                                 | :heavy_minus_sign:                                                                                       | Account key                                                                                              |
| `body`                                                                                                   | [operations.CreateJournalEntryRequestBody](../../models/operations/create-journal-entry-request-body.md) | :heavy_check_mark:                                                                                       | N/A                                                                                                      |