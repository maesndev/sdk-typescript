# CreateEventSubscriptionsRequest

## Example Usage

```typescript
import { CreateEventSubscriptionsRequest } from "maesn/models/operations";

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
| `companyId`                                                                                       | *string*                                                                                          | :heavy_minus_sign:                                                                                | N/A                                                                                               |
| `body`                                                                                            | [models.CreateEventSubscriptionRequestDto](../../models/create-event-subscription-request-dto.md) | :heavy_check_mark:                                                                                | N/A                                                                                               |