# SetEndUserSelectionsRequest

## Example Usage

```typescript
import { SetEndUserSelectionsRequest } from "@maesn/typescript-sdk/models/operations";

let value: SetEndUserSelectionsRequest = {
  accountKey: "<value>",
  environmentName: "<value>",
  companyId: "<id>",
};
```

## Fields

| Field                                                                                          | Type                                                                                           | Required                                                                                       | Description                                                                                    |
| ---------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------- |
| `accountKey`                                                                                   | *string*                                                                                       | :heavy_check_mark:                                                                             | End user account key (X-ACCOUNT-KEY) identifying the end user whose selections are being saved |
| `environmentName`                                                                              | *string*                                                                                       | :heavy_check_mark:                                                                             | Environment name (required for multi-environment systems such as Business Central)             |
| `companyId`                                                                                    | *string*                                                                                       | :heavy_check_mark:                                                                             | ID of the company (required for multi-company target systems)                                  |