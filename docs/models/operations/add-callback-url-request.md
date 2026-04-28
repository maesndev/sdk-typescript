# AddCallbackUrlRequest

## Example Usage

```typescript
import { AddCallbackUrlRequest } from "@maesn/typescript-sdk/models/operations";

let value: AddCallbackUrlRequest = {
  body: {
    callbackUrl: "https://rotating-jacket.com",
    cancelCallbackUrl: "https://pure-order.biz",
  },
};
```

## Fields

| Field                                                                              | Type                                                                               | Required                                                                           | Description                                                                        |
| ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- |
| `apiKey`                                                                           | *string*                                                                           | :heavy_minus_sign:                                                                 | API key                                                                            |
| `accountKey`                                                                       | *string*                                                                           | :heavy_minus_sign:                                                                 | Account key                                                                        |
| `body`                                                                             | [models.CallbackUrlRegistrationDto](../../models/callback-url-registration-dto.md) | :heavy_check_mark:                                                                 | N/A                                                                                |