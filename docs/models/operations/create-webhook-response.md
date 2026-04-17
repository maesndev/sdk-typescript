# CreateWebhookResponse

Webhook created successfully

## Example Usage

```typescript
import { CreateWebhookResponse } from "@maesn/typescript-sdk/models/operations";

let value: CreateWebhookResponse = {
  data: {
    id: "<id>",
    createdDate: "<value>",
    expiresDate: "<value>",
    updatedDate: "<value>",
    callbackUrl: "https://unimportant-almighty.net",
  },
  errors: null,
  rawData: {},
};
```

## Fields

| Field                                                                                 | Type                                                                                  | Required                                                                              | Description                                                                           |
| ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- |
| `meta`                                                                                | [operations.CreateWebhookMeta](../../models/operations/create-webhook-meta.md)        | :heavy_minus_sign:                                                                    | N/A                                                                                   |
| `data`                                                                                | [models.WebhookResponseDto](../../models/webhook-response-dto.md)                     | :heavy_check_mark:                                                                    | N/A                                                                                   |
| `errors`                                                                              | [operations.CreateWebhookErrors](../../models/operations/create-webhook-errors.md)    | :heavy_check_mark:                                                                    | N/A                                                                                   |
| `rawData`                                                                             | [operations.CreateWebhookRawData](../../models/operations/create-webhook-raw-data.md) | :heavy_check_mark:                                                                    | N/A                                                                                   |