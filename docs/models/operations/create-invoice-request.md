# CreateInvoiceRequest

## Example Usage

```typescript
import { CreateInvoiceRequest } from "@maesn/typescript-sdk/models/operations";

let value: CreateInvoiceRequest = {
  body: {
    invoiceDate: "<value>",
    lineItems: [
      {
        quantity: 6737.1,
      },
    ],
  },
};
```

## Fields

| Field                                                                        | Type                                                                         | Required                                                                     | Description                                                                  |
| ---------------------------------------------------------------------------- | ---------------------------------------------------------------------------- | ---------------------------------------------------------------------------- | ---------------------------------------------------------------------------- |
| `environmentName`                                                            | *string*                                                                     | :heavy_minus_sign:                                                           | N/A                                                                          |
| `companyId`                                                                  | *string*                                                                     | :heavy_minus_sign:                                                           | N/A                                                                          |
| `body`                                                                       | [models.CreateInvoiceRequestDto](../../models/create-invoice-request-dto.md) | :heavy_check_mark:                                                           | N/A                                                                          |