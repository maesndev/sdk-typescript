# CreateBookingProposalRequest

## Example Usage

```typescript
import { CreateBookingProposalRequest } from "@maesn/typescript-sdk/models/operations";

let value: CreateBookingProposalRequest = {
  body: {},
};
```

## Fields

| Field                                                                                                          | Type                                                                                                           | Required                                                                                                       | Description                                                                                                    |
| -------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------- |
| `companyId`                                                                                                    | *string*                                                                                                       | :heavy_minus_sign:                                                                                             | ID of the company (required for multi-company target systems)                                                  |
| `apiKey`                                                                                                       | *string*                                                                                                       | :heavy_minus_sign:                                                                                             | API key                                                                                                        |
| `accountKey`                                                                                                   | *string*                                                                                                       | :heavy_minus_sign:                                                                                             | Account key                                                                                                    |
| `body`                                                                                                         | [operations.CreateBookingProposalRequestBody](../../models/operations/create-booking-proposal-request-body.md) | :heavy_check_mark:                                                                                             | N/A                                                                                                            |