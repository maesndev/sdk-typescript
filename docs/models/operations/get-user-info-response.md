# GetUserInfoResponse

## Example Usage

```typescript
import { GetUserInfoResponse } from "@maesn/typescript-sdk/models/operations";

let value: GetUserInfoResponse = {
  data: {
    id: "<id>",
    accountId: "<id>",
    familyName: "<value>",
    name: null,
  },
  errors: {},
  rawData: {},
};
```

## Fields

| Field                                                                              | Type                                                                               | Required                                                                           | Description                                                                        |
| ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- |
| `meta`                                                                             | [operations.GetUserInfoMeta](../../models/operations/get-user-info-meta.md)        | :heavy_minus_sign:                                                                 | N/A                                                                                |
| `data`                                                                             | [models.UserInfoResponseDto](../../models/user-info-response-dto.md)               | :heavy_check_mark:                                                                 | N/A                                                                                |
| `errors`                                                                           | [operations.GetUserInfoErrors](../../models/operations/get-user-info-errors.md)    | :heavy_check_mark:                                                                 | N/A                                                                                |
| `rawData`                                                                          | [operations.GetUserInfoRawData](../../models/operations/get-user-info-raw-data.md) | :heavy_check_mark:                                                                 | N/A                                                                                |