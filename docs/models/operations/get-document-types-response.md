# GetDocumentTypesResponse

List of document types supported by the authenticated end user's connected target system

## Example Usage

```typescript
import { GetDocumentTypesResponse } from "@maesn/typescript-sdk/models/operations";

let value: GetDocumentTypesResponse = {
  data: [],
  errors: {},
  rawData: {},
};
```

## Fields

| Field                                                                                        | Type                                                                                         | Required                                                                                     | Description                                                                                  |
| -------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------- |
| `meta`                                                                                       | [operations.GetDocumentTypesMeta](../../models/operations/get-document-types-meta.md)        | :heavy_minus_sign:                                                                           | N/A                                                                                          |
| `data`                                                                                       | [models.DocumentTypesResponseDto](../../models/document-types-response-dto.md)[]             | :heavy_check_mark:                                                                           | N/A                                                                                          |
| `errors`                                                                                     | [operations.GetDocumentTypesErrors](../../models/operations/get-document-types-errors.md)    | :heavy_check_mark:                                                                           | N/A                                                                                          |
| `rawData`                                                                                    | [operations.GetDocumentTypesRawData](../../models/operations/get-document-types-raw-data.md) | :heavy_check_mark:                                                                           | N/A                                                                                          |