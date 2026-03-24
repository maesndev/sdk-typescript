# GetDocumentExtensionsResponse

## Example Usage

```typescript
import { GetDocumentExtensionsResponse } from "maesn/models/operations";

let value: GetDocumentExtensionsResponse = {
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
    allowedFileExtensions: [
      "<value 1>",
      "<value 2>",
      "<value 3>",
    ],
  },
  errors: {},
  rawData: {},
};
```

## Fields

| Field                                                                                                  | Type                                                                                                   | Required                                                                                               | Description                                                                                            |
| ------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------ |
| `meta`                                                                                                 | [models.MetaResponse](../../models/meta-response.md)                                                   | :heavy_check_mark:                                                                                     | N/A                                                                                                    |
| `data`                                                                                                 | [models.DocumentExtensionsResponseDto](../../models/document-extensions-response-dto.md)               | :heavy_check_mark:                                                                                     | N/A                                                                                                    |
| `errors`                                                                                               | [operations.GetDocumentExtensionsErrors](../../models/operations/get-document-extensions-errors.md)    | :heavy_check_mark:                                                                                     | N/A                                                                                                    |
| `rawData`                                                                                              | [operations.GetDocumentExtensionsRawData](../../models/operations/get-document-extensions-raw-data.md) | :heavy_check_mark:                                                                                     | N/A                                                                                                    |