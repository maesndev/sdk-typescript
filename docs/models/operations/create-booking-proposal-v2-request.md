# CreateBookingProposalV2Request

## Example Usage

```typescript
import { CreateBookingProposalV2Request } from "@maesn/typescript-sdk/models/operations";

let value: CreateBookingProposalV2Request = {
  body: {},
};
```

## Fields

| Field                                                                                                               | Type                                                                                                                | Required                                                                                                            | Description                                                                                                         |
| ------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------- |
| `companyId`                                                                                                         | *string*                                                                                                            | :heavy_minus_sign:                                                                                                  | ID of the company (required for multi-company target systems)                                                       |
| `body`                                                                                                              | [operations.CreateBookingProposalV2RequestBody](../../models/operations/create-booking-proposal-v2-request-body.md) | :heavy_check_mark:                                                                                                  | N/A                                                                                                                 |