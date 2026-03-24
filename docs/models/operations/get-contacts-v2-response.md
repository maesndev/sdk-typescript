# GetContactsV2Response

## Example Usage

```typescript
import { GetContactsV2Response } from "maesn/models/operations";

let value: GetContactsV2Response = {
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
  data: [],
  errors: {},
  rawData: {},
};
```

## Fields

| Field                                                                                  | Type                                                                                   | Required                                                                               | Description                                                                            |
| -------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------- |
| `meta`                                                                                 | [models.MetaResponse](../../models/meta-response.md)                                   | :heavy_check_mark:                                                                     | N/A                                                                                    |
| `data`                                                                                 | [models.ContactResponseDtoV2](../../models/contact-response-dto-v2.md)[]               | :heavy_check_mark:                                                                     | N/A                                                                                    |
| `errors`                                                                               | [operations.GetContactsV2Errors](../../models/operations/get-contacts-v2-errors.md)    | :heavy_check_mark:                                                                     | N/A                                                                                    |
| `rawData`                                                                              | [operations.GetContactsV2RawData](../../models/operations/get-contacts-v2-raw-data.md) | :heavy_check_mark:                                                                     | N/A                                                                                    |