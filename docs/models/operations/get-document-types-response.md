# GetDocumentTypesResponse

## Example Usage

```typescript
import { GetDocumentTypesResponse } from "maesn/models/operations";

let value: GetDocumentTypesResponse = {
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

| Field                                                                                        | Type                                                                                         | Required                                                                                     | Description                                                                                  |
| -------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------- |
| `meta`                                                                                       | [models.MetaResponse](../../models/meta-response.md)                                         | :heavy_check_mark:                                                                           | N/A                                                                                          |
| `data`                                                                                       | [models.DocumentTypesResponseDto](../../models/document-types-response-dto.md)[]             | :heavy_check_mark:                                                                           | N/A                                                                                          |
| `errors`                                                                                     | [operations.GetDocumentTypesErrors](../../models/operations/get-document-types-errors.md)    | :heavy_check_mark:                                                                           | N/A                                                                                          |
| `rawData`                                                                                    | [operations.GetDocumentTypesRawData](../../models/operations/get-document-types-raw-data.md) | :heavy_check_mark:                                                                           | N/A                                                                                          |