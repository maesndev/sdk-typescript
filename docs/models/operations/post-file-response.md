# PostFileResponse

## Example Usage

```typescript
import { PostFileResponse } from "maesn/models/operations";

let value: PostFileResponse = {
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
    base64Encoded: false,
    content: "<value>",
    contentType: "<value>",
    fileName: "example.file",
  },
  errors: {},
  rawData: {},
};
```

## Fields

| Field                                                                       | Type                                                                        | Required                                                                    | Description                                                                 |
| --------------------------------------------------------------------------- | --------------------------------------------------------------------------- | --------------------------------------------------------------------------- | --------------------------------------------------------------------------- |
| `meta`                                                                      | [models.MetaResponse](../../models/meta-response.md)                        | :heavy_check_mark:                                                          | N/A                                                                         |
| `data`                                                                      | [models.DocumentResponseDto](../../models/document-response-dto.md)         | :heavy_check_mark:                                                          | N/A                                                                         |
| `errors`                                                                    | [operations.PostFileErrors](../../models/operations/post-file-errors.md)    | :heavy_check_mark:                                                          | N/A                                                                         |
| `rawData`                                                                   | [operations.PostFileRawData](../../models/operations/post-file-raw-data.md) | :heavy_check_mark:                                                          | N/A                                                                         |