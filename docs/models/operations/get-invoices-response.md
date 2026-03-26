# GetInvoicesResponse

## Example Usage

```typescript
import { GetInvoicesResponse } from "@maesn/typescript-sdk/models/operations";

let value: GetInvoicesResponse = {
  data: [],
  errors: {},
  rawData: {},
};
```

## Fields

| Field                                                                             | Type                                                                              | Required                                                                          | Description                                                                       |
| --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- |
| `meta`                                                                            | [operations.GetInvoicesMeta](../../models/operations/get-invoices-meta.md)        | :heavy_minus_sign:                                                                | N/A                                                                               |
| `data`                                                                            | [models.InvoiceResponseDto](../../models/invoice-response-dto.md)[]               | :heavy_check_mark:                                                                | N/A                                                                               |
| `errors`                                                                          | [operations.GetInvoicesErrors](../../models/operations/get-invoices-errors.md)    | :heavy_check_mark:                                                                | N/A                                                                               |
| `rawData`                                                                         | [operations.GetInvoicesRawData](../../models/operations/get-invoices-raw-data.md) | :heavy_check_mark:                                                                | N/A                                                                               |