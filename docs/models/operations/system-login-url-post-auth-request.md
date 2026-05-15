# SystemLoginUrlPostAuthRequest

## Example Usage

```typescript
import { SystemLoginUrlPostAuthRequest } from "@maesn/typescript-sdk/models/operations";

let value: SystemLoginUrlPostAuthRequest = {
  targetSystem: "<value>",
  body: {},
};
```

## Fields

| Field                                                                                 | Type                                                                                  | Required                                                                              | Description                                                                           |
| ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- |
| `targetSystem`                                                                        | *string*                                                                              | :heavy_check_mark:                                                                    | N/A                                                                                   |
| `apiKey`                                                                              | *string*                                                                              | :heavy_minus_sign:                                                                    | API key                                                                               |
| `accountKey`                                                                          | *string*                                                                              | :heavy_minus_sign:                                                                    | Account key                                                                           |
| `body`                                                                                | [models.CreateAuthWebhookRequestDto](../../models/create-auth-webhook-request-dto.md) | :heavy_check_mark:                                                                    | N/A                                                                                   |