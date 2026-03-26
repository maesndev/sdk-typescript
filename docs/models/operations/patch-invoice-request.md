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

| Field                                                                      | Type                                                                       | Required                                                                   | Description                                                                |
| -------------------------------------------------------------------------- | -------------------------------------------------------------------------- | -------------------------------------------------------------------------- | -------------------------------------------------------------------------- |
| `invoiceId`                                                                | *string*                                                                   | :heavy_check_mark:                                                         | N/A                                                                        |
| `environmentName`                                                          | *string*                                                                   | :heavy_minus_sign:                                                         | N/A                                                                        |
| `companyId`                                                                | *string*                                                                   | :heavy_minus_sign:                                                         | N/A                                                                        |
| `body`                                                                     | [models.PatchInvoiceRequestDto](../../models/patch-invoice-request-dto.md) | :heavy_check_mark:                                                         | N/A                                                                        |