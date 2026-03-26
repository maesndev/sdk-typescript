# GetInvoiceDocumentResponse

## Example Usage

```typescript
import { GetInvoiceDocumentResponse } from "@maesn/typescript-sdk/models/operations";

let value: GetInvoiceDocumentResponse = {
  data: {
    id: "<id>",
    base64Encoded: true,
    content: "<value>",
    contentType: "<value>",
    fileName: "example.file",
  },
  errors: {},
  rawData: null,
};
```

## Fields

| Field                                                                                            | Type                                                                                             | Required                                                                                         | Description                                                                                      |
| ------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------ |
| `meta`                                                                                           | [operations.GetInvoiceDocumentMeta](../../models/operations/get-invoice-document-meta.md)        | :heavy_minus_sign:                                                                               | N/A                                                                                              |
| `data`                                                                                           | [models.DocumentResponseDto](../../models/document-response-dto.md)                              | :heavy_check_mark:                                                                               | N/A                                                                                              |
| `errors`                                                                                         | [operations.GetInvoiceDocumentErrors](../../models/operations/get-invoice-document-errors.md)    | :heavy_check_mark:                                                                               | N/A                                                                                              |
| `rawData`                                                                                        | [operations.GetInvoiceDocumentRawData](../../models/operations/get-invoice-document-raw-data.md) | :heavy_check_mark:                                                                               | N/A                                                                                              |