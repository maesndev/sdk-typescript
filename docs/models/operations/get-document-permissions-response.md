# GetDocumentPermissionsResponse

Permissions for file/document storage for the authenticated end user's connected target system

## Example Usage

```typescript
import { GetDocumentPermissionsResponse } from "@maesn/typescript-sdk/models/operations";

let value: GetDocumentPermissionsResponse = {
  data: {
    isDocumentStorageEnabled: null,
  },
  errors: null,
  rawData: null,
};
```

## Fields

| Field                                                                                                    | Type                                                                                                     | Required                                                                                                 | Description                                                                                              |
| -------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------- |
| `meta`                                                                                                   | [operations.GetDocumentPermissionsMeta](../../models/operations/get-document-permissions-meta.md)        | :heavy_minus_sign:                                                                                       | N/A                                                                                                      |
| `data`                                                                                                   | [models.DocumentPermissionsResponseDto](../../models/document-permissions-response-dto.md)               | :heavy_check_mark:                                                                                       | N/A                                                                                                      |
| `errors`                                                                                                 | [operations.GetDocumentPermissionsErrors](../../models/operations/get-document-permissions-errors.md)    | :heavy_check_mark:                                                                                       | N/A                                                                                                      |
| `rawData`                                                                                                | [operations.GetDocumentPermissionsRawData](../../models/operations/get-document-permissions-raw-data.md) | :heavy_check_mark:                                                                                       | N/A                                                                                                      |