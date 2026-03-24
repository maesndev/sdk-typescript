# GetInvoicesResponse

## Example Usage

```typescript
import { GetInvoicesResponse } from "maesn/models/operations";

let value: GetInvoicesResponse = {
  meta: {
    warnings: [
      "<value 1>",
      "<value 2>",
    ],
    pagination: {
      total: 3438.77,
      perPage: 5109.63,
      currentPage: 2626.79,
      totalPages: 3561.84,
    },
  },
  data: [],
  errors: {},
  rawData: {},
};
```

## Fields

| Field                                                                             | Type                                                                              | Required                                                                          | Description                                                                       |
| --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- |
| `meta`                                                                            | [models.MetaResponse](../../models/meta-response.md)                              | :heavy_check_mark:                                                                | N/A                                                                               |
| `data`                                                                            | [models.InvoiceResponseDto](../../models/invoice-response-dto.md)[]               | :heavy_check_mark:                                                                | N/A                                                                               |
| `errors`                                                                          | [operations.GetInvoicesErrors](../../models/operations/get-invoices-errors.md)    | :heavy_check_mark:                                                                | N/A                                                                               |
| `rawData`                                                                         | [operations.GetInvoicesRawData](../../models/operations/get-invoices-raw-data.md) | :heavy_check_mark:                                                                | N/A                                                                               |