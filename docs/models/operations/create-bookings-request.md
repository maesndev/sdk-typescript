# CreateBookingsRequest

## Example Usage

```typescript
import { CreateBookingsRequest } from "@maesn/typescript-sdk/models/operations";

let value: CreateBookingsRequest = {
  body: {},
};
```

## Fields

| Field                                                                          | Type                                                                           | Required                                                                       | Description                                                                    |
| ------------------------------------------------------------------------------ | ------------------------------------------------------------------------------ | ------------------------------------------------------------------------------ | ------------------------------------------------------------------------------ |
| `companyId`                                                                    | *string*                                                                       | :heavy_minus_sign:                                                             | ID of the company (required for multi-company target systems)                  |
| `body`                                                                         | [models.CreateBookingsRequestDto](../../models/create-bookings-request-dto.md) | :heavy_check_mark:                                                             | N/A                                                                            |