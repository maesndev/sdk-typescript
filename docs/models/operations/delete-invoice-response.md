# DeleteInvoiceResponse

Invoice deleted successfully

## Example Usage

```typescript
import { DeleteInvoiceResponse } from "@maesn/typescript-sdk/models/operations";

let value: DeleteInvoiceResponse = {
  data: {},
  errors: {},
  rawData: {},
};
```

## Fields

| Field                                                                                 | Type                                                                                  | Required                                                                              | Description                                                                           |
| ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- |
| `meta`                                                                                | [operations.DeleteInvoiceMeta](../../models/operations/delete-invoice-meta.md)        | :heavy_minus_sign:                                                                    | N/A                                                                                   |
| `data`                                                                                | [operations.DeleteInvoiceData](../../models/operations/delete-invoice-data.md)        | :heavy_check_mark:                                                                    | N/A                                                                                   |
| `errors`                                                                              | [operations.DeleteInvoiceErrors](../../models/operations/delete-invoice-errors.md)    | :heavy_check_mark:                                                                    | N/A                                                                                   |
| `rawData`                                                                             | [operations.DeleteInvoiceRawData](../../models/operations/delete-invoice-raw-data.md) | :heavy_check_mark:                                                                    | N/A                                                                                   |