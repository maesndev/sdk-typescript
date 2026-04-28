# GetExpenseRequest

## Example Usage

```typescript
import { GetExpenseRequest } from "@maesn/typescript-sdk/models/operations";

let value: GetExpenseRequest = {
  expenseId: "<id>",
};
```

## Fields

| Field                                                                       | Type                                                                        | Required                                                                    | Description                                                                 |
| --------------------------------------------------------------------------- | --------------------------------------------------------------------------- | --------------------------------------------------------------------------- | --------------------------------------------------------------------------- |
| `expenseId`                                                                 | *string*                                                                    | :heavy_check_mark:                                                          | N/A                                                                         |
| `companyId`                                                                 | *string*                                                                    | :heavy_minus_sign:                                                          | ID of the company (required for multi-company target systems)               |
| `journalCode`                                                               | *string*                                                                    | :heavy_minus_sign:                                                          | Journal code used to scope the expense lookup on systems that require it    |
| `rawData`                                                                   | *boolean*                                                                   | :heavy_minus_sign:                                                          | When true, returns the unprocessed response from the upstream target system |
| `apiKey`                                                                    | *string*                                                                    | :heavy_minus_sign:                                                          | API key                                                                     |
| `accountKey`                                                                | *string*                                                                    | :heavy_minus_sign:                                                          | Account key                                                                 |