# CreateWebhookEndUserResponse

Webhook created successfully

## Example Usage

```typescript
import { CreateWebhookEndUserResponse } from "@maesn/typescript-sdk/models/operations";

let value: CreateWebhookEndUserResponse = {
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

| Field                                                                                                 | Type                                                                                                  | Required                                                                                              | Description                                                                                           |
| ----------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------- |
| `meta`                                                                                                | [operations.CreateWebhookEndUserMeta](../../models/operations/create-webhook-end-user-meta.md)        | :heavy_minus_sign:                                                                                    | N/A                                                                                                   |
| `data`                                                                                                | [models.WebhookResponseDto](../../models/webhook-response-dto.md)                                     | :heavy_check_mark:                                                                                    | N/A                                                                                                   |
| `errors`                                                                                              | [operations.CreateWebhookEndUserErrors](../../models/operations/create-webhook-end-user-errors.md)    | :heavy_check_mark:                                                                                    | N/A                                                                                                   |
| `rawData`                                                                                             | [operations.CreateWebhookEndUserRawData](../../models/operations/create-webhook-end-user-raw-data.md) | :heavy_check_mark:                                                                                    | N/A                                                                                                   |