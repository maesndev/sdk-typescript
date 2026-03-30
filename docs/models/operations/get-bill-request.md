# GetBillRequest

## Example Usage

```typescript
import { GetBillRequest } from "@maesn/typescript-sdk/models/operations";

let value: GetBillRequest = {
  billId: "<id>",
};
```

## Fields

| Field                                                                              | Type                                                                               | Required                                                                           | Description                                                                        |
| ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- |
| `billId`                                                                           | *string*                                                                           | :heavy_check_mark:                                                                 | N/A                                                                                |
| `environmentName`                                                                  | *string*                                                                           | :heavy_minus_sign:                                                                 | Environment name (required for multi-environment systems such as Business Central) |
| `companyId`                                                                        | *string*                                                                           | :heavy_minus_sign:                                                                 | ID of the company (required for multi-company target systems)                      |
| `rawData`                                                                          | *boolean*                                                                          | :heavy_minus_sign:                                                                 | When true, returns the unprocessed response from the upstream target system        |