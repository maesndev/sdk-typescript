# GetBillDocumentResponse

## Example Usage

```typescript
import { GetBillDocumentResponse } from "@maesn/typescript-sdk/models/operations";

let value: GetBillDocumentResponse = {
  data: {
    id: "<id>",
    base64Encoded: true,
    content: "<value>",
    contentType: "<value>",
    fileName: "example.file",
  },
  errors: null,
  rawData: {},
};
```

## Fields

| Field                                                                                      | Type                                                                                       | Required                                                                                   | Description                                                                                |
| ------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------ |
| `meta`                                                                                     | [operations.GetBillDocumentMeta](../../models/operations/get-bill-document-meta.md)        | :heavy_minus_sign:                                                                         | N/A                                                                                        |
| `data`                                                                                     | [models.DocumentResponseDto](../../models/document-response-dto.md)                        | :heavy_check_mark:                                                                         | N/A                                                                                        |
| `errors`                                                                                   | [operations.GetBillDocumentErrors](../../models/operations/get-bill-document-errors.md)    | :heavy_check_mark:                                                                         | N/A                                                                                        |
| `rawData`                                                                                  | [operations.GetBillDocumentRawData](../../models/operations/get-bill-document-raw-data.md) | :heavy_check_mark:                                                                         | N/A                                                                                        |