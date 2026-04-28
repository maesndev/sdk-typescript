# CreateEventSubscriptionsRequest

## Example Usage

```typescript
import { CreateEventSubscriptionsRequest } from "@maesn/typescript-sdk/models/operations";

let value: CreateEventSubscriptionsRequest = {
  body: {
    eventType: "<value>",
    callbackUrl: "https://any-tuxedo.com",
  },
};
```

## Fields

| Field                                                                                             | Type                                                                                              | Required                                                                                          | Description                                                                                       |
| ------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------- |
| `companyId`                                                                                       | *string*                                                                                          | :heavy_minus_sign:                                                                                | ID of the company (required for multi-company target systems)                                     |
| `apiKey`                                                                                          | *string*                                                                                          | :heavy_minus_sign:                                                                                | API key                                                                                           |
| `accountKey`                                                                                      | *string*                                                                                          | :heavy_minus_sign:                                                                                | Account key                                                                                       |
| `body`                                                                                            | [models.CreateEventSubscriptionRequestDto](../../models/create-event-subscription-request-dto.md) | :heavy_check_mark:                                                                                | N/A                                                                                               |