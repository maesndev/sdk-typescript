# GetJournalEntriesRequest

## Example Usage

```typescript
import { GetJournalEntriesRequest } from "@maesn/typescript-sdk/models/operations";

let value: GetJournalEntriesRequest = {};
```

## Fields

| Field                                                                              | Type                                                                               | Required                                                                           | Description                                                                        |
| ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- |
| `page`                                                                             | *number*                                                                           | :heavy_minus_sign:                                                                 | N/A                                                                                |
| `limit`                                                                            | *number*                                                                           | :heavy_minus_sign:                                                                 | N/A                                                                                |
| `lastModifiedAt`                                                                   | *string*                                                                           | :heavy_minus_sign:                                                                 | ISO 8601 timestamp; only records modified after this date are returned             |
| `environmentName`                                                                  | *string*                                                                           | :heavy_minus_sign:                                                                 | Environment name (required for multi-environment systems such as Business Central) |
| `companyId`                                                                        | *string*                                                                           | :heavy_minus_sign:                                                                 | ID of the company (required for multi-company target systems)                      |
| `rawData`                                                                          | *boolean*                                                                          | :heavy_minus_sign:                                                                 | When true, returns the unprocessed response from the upstream target system        |
| `fiscalYear`                                                                       | *number*                                                                           | :heavy_minus_sign:                                                                 | Fiscal year to scope the journal entries (e.g. 2024)                               |
| `fiscalYearStartDate`                                                              | *string*                                                                           | :heavy_minus_sign:                                                                 | ISO 8601 start date of the fiscal year used for scoping results                    |