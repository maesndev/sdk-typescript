# GetPaymentTermsRequest

## Example Usage

```typescript
import { GetPaymentTermsRequest } from "@maesn/typescript-sdk/models/operations";

let value: GetPaymentTermsRequest = {};
```

## Fields

| Field                                                                                 | Type                                                                                  | Required                                                                              | Description                                                                           |
| ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- |
| `page`                                                                                | *number*                                                                              | :heavy_minus_sign:                                                                    | N/A                                                                                   |
| `limit`                                                                               | [operations.GetPaymentTermsLimit](../../models/operations/get-payment-terms-limit.md) | :heavy_minus_sign:                                                                    | N/A                                                                                   |
| `lastModifiedAt`                                                                      | *string*                                                                              | :heavy_minus_sign:                                                                    | ISO 8601 timestamp; only records modified after this date are returned                |
| `environmentName`                                                                     | *string*                                                                              | :heavy_minus_sign:                                                                    | Environment name (required for multi-environment systems such as Business Central)    |
| `companyId`                                                                           | *string*                                                                              | :heavy_minus_sign:                                                                    | ID of the company (required for multi-company target systems)                         |
| `rawData`                                                                             | *boolean*                                                                             | :heavy_minus_sign:                                                                    | When true, returns the unprocessed response from the upstream target system           |
| `fiscalYear`                                                                          | *number*                                                                              | :heavy_minus_sign:                                                                    | Fiscal year to scope the payment terms results (e.g. 2024)                            |
| `fiscalYearStartDate`                                                                 | *string*                                                                              | :heavy_minus_sign:                                                                    | ISO 8601 start date of the fiscal year used for scoping results                       |
| `apiKey`                                                                              | *string*                                                                              | :heavy_minus_sign:                                                                    | API key                                                                               |
| `accountKey`                                                                          | *string*                                                                              | :heavy_minus_sign:                                                                    | Account key                                                                           |