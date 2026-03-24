# ContactByBatchMetaDataResponseDto

## Example Usage

```typescript
import { ContactByBatchMetaDataResponseDto } from "maesn/models";

let value: ContactByBatchMetaDataResponseDto = {
  id: "<id>",
  accountNumberLength: 9934.97,
  chartOfAccount: "<value>",
  createdDate: "<value>",
  entries: [],
  fiscalYearStartDate: "<value>",
  taskId: "<id>",
};
```

## Fields

| Field                                                            | Type                                                             | Required                                                         | Description                                                      |
| ---------------------------------------------------------------- | ---------------------------------------------------------------- | ---------------------------------------------------------------- | ---------------------------------------------------------------- |
| `id`                                                             | *string*                                                         | :heavy_check_mark:                                               | N/A                                                              |
| `accountNumberLength`                                            | *number*                                                         | :heavy_check_mark:                                               | N/A                                                              |
| `chartOfAccount`                                                 | *string*                                                         | :heavy_check_mark:                                               | N/A                                                              |
| `createdDate`                                                    | *string*                                                         | :heavy_check_mark:                                               | N/A                                                              |
| `entries`                                                        | [models.ContactResponseDto](../models/contact-response-dto.md)[] | :heavy_check_mark:                                               | N/A                                                              |
| `fiscalYearStartDate`                                            | *string*                                                         | :heavy_check_mark:                                               | N/A                                                              |
| `taskId`                                                         | *string*                                                         | :heavy_check_mark:                                               | N/A                                                              |