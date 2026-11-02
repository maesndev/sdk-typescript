# UpdateBookingProposalAsyncRequest

## Example Usage

```typescript
import { UpdateBookingProposalAsyncRequest } from "@maesn/typescript-sdk/models/operations";

let value: UpdateBookingProposalAsyncRequest = {
  bookingProposalId: "<id>",
  body: {},
};
```

## Fields

| Field                                                                                                                     | Type                                                                                                                      | Required                                                                                                                  | Description                                                                                                               |
| ------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------- |
| `bookingProposalId`                                                                                                       | *string*                                                                                                                  | :heavy_check_mark:                                                                                                        | N/A                                                                                                                       |
| `companyId`                                                                                                               | *string*                                                                                                                  | :heavy_minus_sign:                                                                                                        | ID of the company (required for multi-company target systems)                                                             |
| `apiKey`                                                                                                                  | *string*                                                                                                                  | :heavy_minus_sign:                                                                                                        | API key                                                                                                                   |
| `accountKey`                                                                                                              | *string*                                                                                                                  | :heavy_minus_sign:                                                                                                        | Account key                                                                                                               |
| `body`                                                                                                                    | [operations.UpdateBookingProposalAsyncRequestBody](../../models/operations/update-booking-proposal-async-request-body.md) | :heavy_check_mark:                                                                                                        | N/A                                                                                                                       |