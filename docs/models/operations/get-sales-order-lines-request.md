# GetSalesOrderLinesRequest

## Example Usage

```typescript
import { GetSalesOrderLinesRequest } from "@maesn/typescript-sdk/models/operations";

let value: GetSalesOrderLinesRequest = {
  salesOrderId: "<id>",
};
```

## Fields

| Field                                                                                        | Type                                                                                         | Required                                                                                     | Description                                                                                  |
| -------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------- |
| `salesOrderId`                                                                               | *string*                                                                                     | :heavy_check_mark:                                                                           | N/A                                                                                          |
| `page`                                                                                       | *number*                                                                                     | :heavy_minus_sign:                                                                           | N/A                                                                                          |
| `limit`                                                                                      | [operations.GetSalesOrderLinesLimit](../../models/operations/get-sales-order-lines-limit.md) | :heavy_minus_sign:                                                                           | N/A                                                                                          |
| `lastModifiedAt`                                                                             | *string*                                                                                     | :heavy_minus_sign:                                                                           | ISO 8601 timestamp; only records modified after this date are returned                       |
| `environmentName`                                                                            | *string*                                                                                     | :heavy_minus_sign:                                                                           | Environment name (required for multi-environment systems such as Business Central)           |
| `companyId`                                                                                  | *string*                                                                                     | :heavy_minus_sign:                                                                           | ID of the company (required for multi-company target systems)                                |
| `rawData`                                                                                    | *boolean*                                                                                    | :heavy_minus_sign:                                                                           | When true, returns the unprocessed response from the upstream target system                  |
| `apiKey`                                                                                     | *string*                                                                                     | :heavy_minus_sign:                                                                           | API key                                                                                      |
| `accountKey`                                                                                 | *string*                                                                                     | :heavy_minus_sign:                                                                           | Account key                                                                                  |