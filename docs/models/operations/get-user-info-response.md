# GetUserInfoResponse

## Example Usage

```typescript
import { GetUserInfoResponse } from "maesn/models/operations";

let value: GetUserInfoResponse = {
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
    accountId: "<id>",
    familyName: "<value>",
    name: "<value>",
  },
  errors: {},
  rawData: {},
};
```

## Fields

| Field                                                                              | Type                                                                               | Required                                                                           | Description                                                                        |
| ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- |
| `meta`                                                                             | [models.MetaResponse](../../models/meta-response.md)                               | :heavy_check_mark:                                                                 | N/A                                                                                |
| `data`                                                                             | [models.UserInfoResponseDto](../../models/user-info-response-dto.md)               | :heavy_check_mark:                                                                 | N/A                                                                                |
| `errors`                                                                           | [operations.GetUserInfoErrors](../../models/operations/get-user-info-errors.md)    | :heavy_check_mark:                                                                 | N/A                                                                                |
| `rawData`                                                                          | [operations.GetUserInfoRawData](../../models/operations/get-user-info-raw-data.md) | :heavy_check_mark:                                                                 | N/A                                                                                |