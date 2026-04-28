# GetBillLineItemsRequest

## Example Usage

```typescript
import { GetBillLineItemsRequest } from "@maesn/typescript-sdk/models/operations";

let value: GetBillLineItemsRequest = {
  billId: "<id>",
};
```

## Fields

| Field                                                                       | Type                                                                        | Required                                                                    | Description                                                                 |
| --------------------------------------------------------------------------- | --------------------------------------------------------------------------- | --------------------------------------------------------------------------- | --------------------------------------------------------------------------- |
| `billId`                                                                    | *string*                                                                    | :heavy_check_mark:                                                          | N/A                                                                         |
| `companyId`                                                                 | *string*                                                                    | :heavy_minus_sign:                                                          | ID of the company (required for multi-company target systems)               |
| `rawData`                                                                   | *boolean*                                                                   | :heavy_minus_sign:                                                          | When true, returns the unprocessed response from the upstream target system |
| `apiKey`                                                                    | *string*                                                                    | :heavy_minus_sign:                                                          | API key                                                                     |
| `accountKey`                                                                | *string*                                                                    | :heavy_minus_sign:                                                          | Account key                                                                 |