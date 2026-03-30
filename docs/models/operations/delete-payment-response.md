# DeletePaymentResponse

Operation completed successfully

## Example Usage

```typescript
import { DeletePaymentResponse } from "@maesn/typescript-sdk/models/operations";

let value: DeletePaymentResponse = {
  data: "<value>",
  errors: {},
  rawData: null,
};
```

## Fields

| Field                                                                                 | Type                                                                                  | Required                                                                              | Description                                                                           |
| ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- |
| `meta`                                                                                | [operations.DeletePaymentMeta](../../models/operations/delete-payment-meta.md)        | :heavy_minus_sign:                                                                    | N/A                                                                                   |
| `data`                                                                                | *string*                                                                              | :heavy_check_mark:                                                                    | N/A                                                                                   |
| `errors`                                                                              | [operations.DeletePaymentErrors](../../models/operations/delete-payment-errors.md)    | :heavy_check_mark:                                                                    | N/A                                                                                   |
| `rawData`                                                                             | [operations.DeletePaymentRawData](../../models/operations/delete-payment-raw-data.md) | :heavy_check_mark:                                                                    | N/A                                                                                   |