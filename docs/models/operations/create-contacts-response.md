# CreateContactsResponse

## Example Usage

```typescript
import { CreateContactsResponse } from "@maesn/typescript-sdk/models/operations";

let value: CreateContactsResponse = {
  data: {
    id: "<id>",
    accountNumberLength: 9963.13,
    chartOfAccount: "<value>",
    createdDate: "<value>",
    entries: null,
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
| `meta`                                                                                              | [operations.CreateContactsMeta](../../models/operations/create-contacts-meta.md)                    | :heavy_minus_sign:                                                                                  | N/A                                                                                                 |
| `data`                                                                                              | [models.ContactByBatchMetaDataResponseDto](../../models/contact-by-batch-meta-data-response-dto.md) | :heavy_check_mark:                                                                                  | N/A                                                                                                 |
| `errors`                                                                                            | [operations.CreateContactsErrors](../../models/operations/create-contacts-errors.md)                | :heavy_check_mark:                                                                                  | N/A                                                                                                 |
| `rawData`                                                                                           | [operations.CreateContactsRawData](../../models/operations/create-contacts-raw-data.md)             | :heavy_check_mark:                                                                                  | N/A                                                                                                 |