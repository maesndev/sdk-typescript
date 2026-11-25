# DeleteContactResponse

Contact deleted successfully

## Example Usage

```typescript
import { DeleteContactResponse } from "@maesn/typescript-sdk/models/operations";

let value: DeleteContactResponse = {
  data: {},
  errors: {},
  rawData: null,
};
```

## Fields

| Field                                                                                 | Type                                                                                  | Required                                                                              | Description                                                                           |
| ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- |
| `meta`                                                                                | [operations.DeleteContactMeta](../../models/operations/delete-contact-meta.md)        | :heavy_minus_sign:                                                                    | N/A                                                                                   |
| `data`                                                                                | [operations.DeleteContactData](../../models/operations/delete-contact-data.md)        | :heavy_check_mark:                                                                    | N/A                                                                                   |
| `errors`                                                                              | [operations.DeleteContactErrors](../../models/operations/delete-contact-errors.md)    | :heavy_check_mark:                                                                    | N/A                                                                                   |
| `rawData`                                                                             | [operations.DeleteContactRawData](../../models/operations/delete-contact-raw-data.md) | :heavy_check_mark:                                                                    | N/A                                                                                   |