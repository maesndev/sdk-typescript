# CreateBookingsRequest

## Example Usage

```typescript
import { CreateBookingsRequest } from "maesn/models/operations";

let value: CreateBookingsRequest = {
  body: {
    accountNumberLength: 3843.72,
    chartOfAccount: "SKR03",
    entries: [],
    fiscalYearStartDate: "<value>",
  },
};
```

## Fields

| Field                                                                          | Type                                                                           | Required                                                                       | Description                                                                    |
| ------------------------------------------------------------------------------ | ------------------------------------------------------------------------------ | ------------------------------------------------------------------------------ | ------------------------------------------------------------------------------ |
| `companyId`                                                                    | *string*                                                                       | :heavy_minus_sign:                                                             | N/A                                                                            |
| `body`                                                                         | [models.CreateBookingsRequestDto](../../models/create-bookings-request-dto.md) | :heavy_check_mark:                                                             | N/A                                                                            |