# GetContactsResponse

## Example Usage

```typescript
import { GetContactsResponse } from "maesn/models/operations";

let value: GetContactsResponse = {
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

| Field                                                                             | Type                                                                              | Required                                                                          | Description                                                                       |
| --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- |
| `meta`                                                                            | [models.MetaResponse](../../models/meta-response.md)                              | :heavy_check_mark:                                                                | N/A                                                                               |
| `data`                                                                            | [models.ContactResponseDtoV2](../../models/contact-response-dto-v2.md)[]          | :heavy_check_mark:                                                                | N/A                                                                               |
| `errors`                                                                          | [operations.GetContactsErrors](../../models/operations/get-contacts-errors.md)    | :heavy_check_mark:                                                                | N/A                                                                               |
| `rawData`                                                                         | [operations.GetContactsRawData](../../models/operations/get-contacts-raw-data.md) | :heavy_check_mark:                                                                | N/A                                                                               |