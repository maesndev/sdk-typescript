# PatchBankAccountRequest

## Example Usage

```typescript
import { PatchBankAccountRequest } from "@maesn/typescript-sdk/models/operations";

let value: PatchBankAccountRequest = {
  bankAccountId: "<id>",
  body: {
    balance: 785.82,
    version: 2776.94,
  },
};
```

## Fields

| Field                                                                               | Type                                                                                | Required                                                                            | Description                                                                         |
| ----------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------- |
| `bankAccountId`                                                                     | *string*                                                                            | :heavy_check_mark:                                                                  | N/A                                                                                 |
| `apiKey`                                                                            | *string*                                                                            | :heavy_minus_sign:                                                                  | API key                                                                             |
| `accountKey`                                                                        | *string*                                                                            | :heavy_minus_sign:                                                                  | Account key                                                                         |
| `body`                                                                              | [models.PatchBankAccountRequestDto](../../models/patch-bank-account-request-dto.md) | :heavy_check_mark:                                                                  | N/A                                                                                 |