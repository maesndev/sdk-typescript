# CreateContactsV1Response

## Example Usage

```typescript
import { CreateContactsV1Response } from "@maesn/typescript-sdk/models/operations";

let value: CreateContactsV1Response = {
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
| `meta`                                                                                              | [operations.CreateContactsV1Meta](../../models/operations/create-contacts-v1-meta.md)               | :heavy_minus_sign:                                                                                  | N/A                                                                                                 |
| `data`                                                                                              | [models.ContactByBatchMetaDataResponseDto](../../models/contact-by-batch-meta-data-response-dto.md) | :heavy_check_mark:                                                                                  | N/A                                                                                                 |
| `errors`                                                                                            | [operations.CreateContactsV1Errors](../../models/operations/create-contacts-v1-errors.md)           | :heavy_check_mark:                                                                                  | N/A                                                                                                 |
| `rawData`                                                                                           | [operations.CreateContactsV1RawData](../../models/operations/create-contacts-v1-raw-data.md)        | :heavy_check_mark:                                                                                  | N/A                                                                                                 |