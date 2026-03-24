# CreateContactsResponse

## Example Usage

```typescript
import { CreateContactsResponse } from "maesn/models/operations";

let value: CreateContactsResponse = {
  meta: {
    warnings: [
      "<value 1>",
      "<value 2>",
    ],
    pagination: {
      total: 3438.77,
      perPage: 5109.63,
      currentPage: 2626.79,
      totalPages: 3561.84,
    },
  },
  data: {
    id: "<id>",
    accountNumberLength: 1271.76,
    chartOfAccount: "<value>",
    createdDate: "<value>",
    entries: [],
    fiscalYearStartDate: "<value>",
    taskId: "<id>",
  },
  errors: {},
  rawData: {},
};
```

## Fields

| Field                                                                                               | Type                                                                                                | Required                                                                                            | Description                                                                                         |
| --------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------- |
| `meta`                                                                                              | [models.MetaResponse](../../models/meta-response.md)                                                | :heavy_check_mark:                                                                                  | N/A                                                                                                 |
| `data`                                                                                              | [models.ContactByBatchMetaDataResponseDto](../../models/contact-by-batch-meta-data-response-dto.md) | :heavy_check_mark:                                                                                  | N/A                                                                                                 |
| `errors`                                                                                            | [operations.CreateContactsErrors](../../models/operations/create-contacts-errors.md)                | :heavy_check_mark:                                                                                  | N/A                                                                                                 |
| `rawData`                                                                                           | [operations.CreateContactsRawData](../../models/operations/create-contacts-raw-data.md)             | :heavy_check_mark:                                                                                  | N/A                                                                                                 |