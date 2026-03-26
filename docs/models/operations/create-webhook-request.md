# CreateWebhookRequest

## Example Usage

```typescript
import { CreateWebhookRequest } from "@maesn/typescript-sdk/models/operations";

let value: CreateWebhookRequest = {
  body: {
    callbackUrl: "https://well-worn-stranger.com/",
  },
};
```

## Fields

| Field                                                                                             | Type                                                                                              | Required                                                                                          | Description                                                                                       |
| ------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------- |
| `environmentName`                                                                                 | *string*                                                                                          | :heavy_minus_sign:                                                                                | N/A                                                                                               |
| `companyId`                                                                                       | *string*                                                                                          | :heavy_minus_sign:                                                                                | N/A                                                                                               |
| `body`                                                                                            | [models.CreateAccountingWebhookRequestDto](../../models/create-accounting-webhook-request-dto.md) | :heavy_check_mark:                                                                                | N/A                                                                                               |