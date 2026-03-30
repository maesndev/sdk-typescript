# PatchInvoiceRequest

## Example Usage

```typescript
import { PatchInvoiceRequest } from "@maesn/typescript-sdk/models/operations";

let value: PatchInvoiceRequest = {
  invoiceId: "<id>",
  body: {},
};
```

## Fields

| Field                                                                              | Type                                                                               | Required                                                                           | Description                                                                        |
| ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- |
| `invoiceId`                                                                        | *string*                                                                           | :heavy_check_mark:                                                                 | N/A                                                                                |
| `environmentName`                                                                  | *string*                                                                           | :heavy_minus_sign:                                                                 | Environment name (required for multi-environment systems such as Business Central) |
| `companyId`                                                                        | *string*                                                                           | :heavy_minus_sign:                                                                 | ID of the company (required for multi-company target systems)                      |
| `body`                                                                             | [models.PatchInvoiceRequestDto](../../models/patch-invoice-request-dto.md)         | :heavy_check_mark:                                                                 | N/A                                                                                |