# PostFileResponse

## Example Usage

```typescript
import { PostFileResponse } from "@maesn/typescript-sdk/models/operations";

let value: PostFileResponse = {
  data: {
    id: "<id>",
    base64Encoded: true,
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
| `meta`                                                                      | [operations.PostFileMeta](../../models/operations/post-file-meta.md)        | :heavy_minus_sign:                                                          | N/A                                                                         |
| `data`                                                                      | [models.DocumentResponseDto](../../models/document-response-dto.md)         | :heavy_check_mark:                                                          | N/A                                                                         |
| `errors`                                                                    | [operations.PostFileErrors](../../models/operations/post-file-errors.md)    | :heavy_check_mark:                                                          | N/A                                                                         |
| `rawData`                                                                   | [operations.PostFileRawData](../../models/operations/post-file-raw-data.md) | :heavy_check_mark:                                                          | N/A                                                                         |