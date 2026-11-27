# GetDocumentPermissionsRequest

## Example Usage

```typescript
import { GetDocumentPermissionsRequest } from "@maesn/typescript-sdk/models/operations";

let value: GetDocumentPermissionsRequest = {};
```

## Fields

| Field                                                                       | Type                                                                        | Required                                                                    | Description                                                                 |
| --------------------------------------------------------------------------- | --------------------------------------------------------------------------- | --------------------------------------------------------------------------- | --------------------------------------------------------------------------- |
| `companyId`                                                                 | *string*                                                                    | :heavy_minus_sign:                                                          | ID of the company (required for multi-company target systems)               |
| `rawData`                                                                   | *boolean*                                                                   | :heavy_minus_sign:                                                          | When true, returns the unprocessed response from the upstream target system |
| `apiKey`                                                                    | *string*                                                                    | :heavy_minus_sign:                                                          | API key                                                                     |
| `accountKey`                                                                | *string*                                                                    | :heavy_minus_sign:                                                          | Account key                                                                 |