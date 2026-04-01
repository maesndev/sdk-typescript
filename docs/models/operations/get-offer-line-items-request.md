# GetOfferLineItemsRequest

## Example Usage

```typescript
import { GetOfferLineItemsRequest } from "@maesn/typescript-sdk/models/operations";

let value: GetOfferLineItemsRequest = {
  offerId: "<id>",
};
```

## Fields

| Field                                                                                      | Type                                                                                       | Required                                                                                   | Description                                                                                |
| ------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------ |
| `offerId`                                                                                  | *string*                                                                                   | :heavy_check_mark:                                                                         | N/A                                                                                        |
| `page`                                                                                     | *number*                                                                                   | :heavy_minus_sign:                                                                         | N/A                                                                                        |
| `limit`                                                                                    | [operations.GetOfferLineItemsLimit](../../models/operations/get-offer-line-items-limit.md) | :heavy_minus_sign:                                                                         | N/A                                                                                        |
| `lastModifiedAt`                                                                           | *string*                                                                                   | :heavy_minus_sign:                                                                         | ISO 8601 timestamp; only records modified after this date are returned                     |
| `environmentName`                                                                          | *string*                                                                                   | :heavy_minus_sign:                                                                         | Environment name (required for multi-environment systems such as Business Central)         |
| `companyId`                                                                                | *string*                                                                                   | :heavy_minus_sign:                                                                         | ID of the company (required for multi-company target systems)                              |
| `rawData`                                                                                  | *boolean*                                                                                  | :heavy_minus_sign:                                                                         | When true, returns the unprocessed response from the upstream target system                |