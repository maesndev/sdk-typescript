# CreateJournalEntryRequest

## Example Usage

```typescript
import { CreateJournalEntryRequest } from "@maesn/typescript-sdk/models/operations";

let value: CreateJournalEntryRequest = {
  body: {},
};
```

## Fields

| Field                                                                                                    | Type                                                                                                     | Required                                                                                                 | Description                                                                                              |
| -------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------- |
| `environmentName`                                                                                        | *string*                                                                                                 | :heavy_minus_sign:                                                                                       | Environment name (required for multi-environment systems such as Business Central)                       |
| `companyId`                                                                                              | *string*                                                                                                 | :heavy_minus_sign:                                                                                       | ID of the company (required for multi-company target systems)                                            |
| `apiKey`                                                                                                 | *string*                                                                                                 | :heavy_minus_sign:                                                                                       | API key                                                                                                  |
| `accountKey`                                                                                             | *string*                                                                                                 | :heavy_minus_sign:                                                                                       | Account key                                                                                              |
| `body`                                                                                                   | [operations.CreateJournalEntryRequestBody](../../models/operations/create-journal-entry-request-body.md) | :heavy_check_mark:                                                                                       | N/A                                                                                                      |