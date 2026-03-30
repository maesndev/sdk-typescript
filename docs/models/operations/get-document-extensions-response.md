# GetDocumentExtensionsResponse

List of permitted file extensions for the authenticated end user's connected target system

## Example Usage

```typescript
import { GetDocumentExtensionsResponse } from "@maesn/typescript-sdk/models/operations";

let value: GetDocumentExtensionsResponse = {
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
| `meta`                                                                                                 | [operations.GetDocumentExtensionsMeta](../../models/operations/get-document-extensions-meta.md)        | :heavy_minus_sign:                                                                                     | N/A                                                                                                    |
| `data`                                                                                                 | [models.DocumentExtensionsResponseDto](../../models/document-extensions-response-dto.md)               | :heavy_check_mark:                                                                                     | N/A                                                                                                    |
| `errors`                                                                                               | [operations.GetDocumentExtensionsErrors](../../models/operations/get-document-extensions-errors.md)    | :heavy_check_mark:                                                                                     | N/A                                                                                                    |
| `rawData`                                                                                              | [operations.GetDocumentExtensionsRawData](../../models/operations/get-document-extensions-raw-data.md) | :heavy_check_mark:                                                                                     | N/A                                                                                                    |