# LongTokenRequest

## Example Usage

```typescript
import { LongTokenRequest } from "@maesn/typescript-sdk/models/operations";

let value: LongTokenRequest = {
  targetSystem: "<value>",
  companyId: "<id>",
};
```

## Fields

| Field                                                         | Type                                                          | Required                                                      | Description                                                   |
| ------------------------------------------------------------- | ------------------------------------------------------------- | ------------------------------------------------------------- | ------------------------------------------------------------- |
| `targetSystem`                                                | *string*                                                      | :heavy_check_mark:                                            | Identifier of the target system (e.g. exact, sevdesk, xero)   |
| `companyId`                                                   | *string*                                                      | :heavy_check_mark:                                            | ID of the company (required for multi-company target systems) |
| `callbackUrl`                                                 | *string*                                                      | :heavy_minus_sign:                                            | URL to redirect to after successful authentication            |