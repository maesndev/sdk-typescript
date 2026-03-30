# WebhookResponseDto

## Example Usage

```typescript
import { WebhookResponseDto } from "@maesn/typescript-sdk/models";

let value: WebhookResponseDto = {
  id: "<id>",
  createdDate: "<value>",
  expiresDate: "<value>",
  updatedDate: "<value>",
  callbackUrl: "https://inexperienced-rosemary.com",
};
```

## Fields

| Field              | Type               | Required           | Description        |
| ------------------ | ------------------ | ------------------ | ------------------ |
| `id`               | *string*           | :heavy_check_mark: | N/A                |
| `createdDate`      | *string*           | :heavy_check_mark: | N/A                |
| `expiresDate`      | *string*           | :heavy_check_mark: | N/A                |
| `updatedDate`      | *string*           | :heavy_check_mark: | N/A                |
| `callbackUrl`      | *string*           | :heavy_check_mark: | N/A                |
| `secret`           | *string*           | :heavy_minus_sign: | N/A                |