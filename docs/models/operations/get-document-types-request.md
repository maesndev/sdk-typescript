# GetDocumentTypesRequest

## Example Usage

```typescript
import { GetDocumentTypesRequest } from "@maesn/typescript-sdk/models/operations";

let value: GetDocumentTypesRequest = {};
```

## Fields

| Field                                                                                   | Type                                                                                    | Required                                                                                | Description                                                                             |
| --------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------- |
| `page`                                                                                  | *number*                                                                                | :heavy_minus_sign:                                                                      | N/A                                                                                     |
| `limit`                                                                                 | [operations.GetDocumentTypesLimit](../../models/operations/get-document-types-limit.md) | :heavy_minus_sign:                                                                      | N/A                                                                                     |
| `companyId`                                                                             | *string*                                                                                | :heavy_minus_sign:                                                                      | ID of the company (required for multi-company target systems)                           |
| `rawData`                                                                               | *boolean*                                                                               | :heavy_minus_sign:                                                                      | When true, returns the unprocessed response from the upstream target system             |
| `apiKey`                                                                                | *string*                                                                                | :heavy_minus_sign:                                                                      | API key                                                                                 |
| `accountKey`                                                                            | *string*                                                                                | :heavy_minus_sign:                                                                      | Account key                                                                             |