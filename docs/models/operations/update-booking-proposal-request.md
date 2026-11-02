# UpdateBookingProposalRequest

## Example Usage

```typescript
import { UpdateBookingProposalRequest } from "@maesn/typescript-sdk/models/operations";

let value: UpdateBookingProposalRequest = {
  bookingProposalId: "<id>",
  body: {},
};
```

## Fields

| Field                                                                                                          | Type                                                                                                           | Required                                                                                                       | Description                                                                                                    |
| -------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------- |
| `bookingProposalId`                                                                                            | *string*                                                                                                       | :heavy_check_mark:                                                                                             | N/A                                                                                                            |
| `companyId`                                                                                                    | *string*                                                                                                       | :heavy_minus_sign:                                                                                             | ID of the company (required for multi-company target systems)                                                  |
| `environmentName`                                                                                              | *string*                                                                                                       | :heavy_minus_sign:                                                                                             | Environment name (required for multi-environment systems such as Business Central)                             |
| `apiKey`                                                                                                       | *string*                                                                                                       | :heavy_minus_sign:                                                                                             | API key                                                                                                        |
| `accountKey`                                                                                                   | *string*                                                                                                       | :heavy_minus_sign:                                                                                             | Account key                                                                                                    |
| `body`                                                                                                         | [operations.UpdateBookingProposalRequestBody](../../models/operations/update-booking-proposal-request-body.md) | :heavy_check_mark:                                                                                             | N/A                                                                                                            |