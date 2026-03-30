# CreateWebHookTenantResponse

Webhook created successfully

## Example Usage

```typescript
import { CreateWebHookTenantResponse } from "@maesn/typescript-sdk/models/operations";

let value: CreateWebHookTenantResponse = {
  data: {
    id: "<id>",
    createdDate: "<value>",
    expiresDate: "<value>",
    updatedDate: "<value>",
    callbackUrl: "https://unimportant-almighty.net",
  },
  errors: {},
  rawData: {},
};
```

## Fields

| Field                                                                                               | Type                                                                                                | Required                                                                                            | Description                                                                                         |
| --------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------- |
| `meta`                                                                                              | [operations.CreateWebHookTenantMeta](../../models/operations/create-web-hook-tenant-meta.md)        | :heavy_minus_sign:                                                                                  | N/A                                                                                                 |
| `data`                                                                                              | [models.WebhookResponseDto](../../models/webhook-response-dto.md)                                   | :heavy_check_mark:                                                                                  | N/A                                                                                                 |
| `errors`                                                                                            | [operations.CreateWebHookTenantErrors](../../models/operations/create-web-hook-tenant-errors.md)    | :heavy_check_mark:                                                                                  | N/A                                                                                                 |
| `rawData`                                                                                           | [operations.CreateWebHookTenantRawData](../../models/operations/create-web-hook-tenant-raw-data.md) | :heavy_check_mark:                                                                                  | N/A                                                                                                 |