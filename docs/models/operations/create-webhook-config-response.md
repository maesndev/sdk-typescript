# CreateWebhookConfigResponse

Webhook created successfully

## Example Usage

```typescript
import { CreateWebhookConfigResponse } from "@maesn/typescript-sdk/models/operations";

let value: CreateWebhookConfigResponse = {
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

| Field                                                                                              | Type                                                                                               | Required                                                                                           | Description                                                                                        |
| -------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------- |
| `meta`                                                                                             | [operations.CreateWebhookConfigMeta](../../models/operations/create-webhook-config-meta.md)        | :heavy_minus_sign:                                                                                 | N/A                                                                                                |
| `data`                                                                                             | [models.WebhookResponseDto](../../models/webhook-response-dto.md)                                  | :heavy_check_mark:                                                                                 | N/A                                                                                                |
| `errors`                                                                                           | [operations.CreateWebhookConfigErrors](../../models/operations/create-webhook-config-errors.md)    | :heavy_check_mark:                                                                                 | N/A                                                                                                |
| `rawData`                                                                                          | [operations.CreateWebhookConfigRawData](../../models/operations/create-webhook-config-raw-data.md) | :heavy_check_mark:                                                                                 | N/A                                                                                                |