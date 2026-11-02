# CreateContactAsyncRequest

## Example Usage

```typescript
import { CreateContactAsyncRequest } from "@maesn/typescript-sdk/models/operations";

let value: CreateContactAsyncRequest = {
  body: {
    contactType: "CONTACT_PERSON",
  },
};
```

## Fields

| Field                                                                             | Type                                                                              | Required                                                                          | Description                                                                       |
| --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- |
| `apiKey`                                                                          | *string*                                                                          | :heavy_minus_sign:                                                                | API key                                                                           |
| `accountKey`                                                                      | *string*                                                                          | :heavy_minus_sign:                                                                | Account key                                                                       |
| `body`                                                                            | [models.CreateContactRequestDtoV2](../../models/create-contact-request-dto-v2.md) | :heavy_check_mark:                                                                | N/A                                                                               |