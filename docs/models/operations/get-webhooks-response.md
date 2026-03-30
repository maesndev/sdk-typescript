# GetWebhooksResponse

List of webhooks for the authenticated end user's connected target system

## Example Usage

```typescript
import { GetWebhooksResponse } from "@maesn/typescript-sdk/models/operations";

let value: GetWebhooksResponse = {
  data: [
    {
      id: "<id>",
      createdDate: "<value>",
      expiresDate: "<value>",
      updatedDate: "<value>",
      callbackUrl: "https://crushing-equal.info/",
    },
  ],
  errors: {},
  rawData: {},
};
```

## Fields

| Field                                                                             | Type                                                                              | Required                                                                          | Description                                                                       |
| --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- |
| `meta`                                                                            | [operations.GetWebhooksMeta](../../models/operations/get-webhooks-meta.md)        | :heavy_minus_sign:                                                                | N/A                                                                               |
| `data`                                                                            | [models.WebhookResponseDto](../../models/webhook-response-dto.md)[]               | :heavy_check_mark:                                                                | N/A                                                                               |
| `errors`                                                                          | [operations.GetWebhooksErrors](../../models/operations/get-webhooks-errors.md)    | :heavy_check_mark:                                                                | N/A                                                                               |
| `rawData`                                                                         | [operations.GetWebhooksRawData](../../models/operations/get-webhooks-raw-data.md) | :heavy_check_mark:                                                                | N/A                                                                               |