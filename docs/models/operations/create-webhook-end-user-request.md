# CreateWebhookEndUserRequest

## Example Usage

```typescript
import { CreateWebhookEndUserRequest } from "maesn/models/operations";

let value: CreateWebhookEndUserRequest = {
  body: {
    callbackUrl: "https://well-worn-stranger.com/",
    eventType: "<value>",
    resource: "<value>",
    targetSystem: "<value>",
  },
};
```

## Fields

| Field                                                                        | Type                                                                         | Required                                                                     | Description                                                                  |
| ---------------------------------------------------------------------------- | ---------------------------------------------------------------------------- | ---------------------------------------------------------------------------- | ---------------------------------------------------------------------------- |
| `environmentName`                                                            | *string*                                                                     | :heavy_minus_sign:                                                           | N/A                                                                          |
| `companyId`                                                                  | *string*                                                                     | :heavy_minus_sign:                                                           | N/A                                                                          |
| `body`                                                                       | [models.CreateWebhookRequestDto](../../models/create-webhook-request-dto.md) | :heavy_check_mark:                                                           | N/A                                                                          |