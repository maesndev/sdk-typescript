# GetContactsV2Response

List of contacts for the authenticated end user's connected target system

## Example Usage

```typescript
import { GetContactsV2Response } from "@maesn/typescript-sdk/models/operations";

let value: GetContactsV2Response = {
  data: [],
  errors: null,
  rawData: {},
};
```

## Fields

| Field                                                                                  | Type                                                                                   | Required                                                                               | Description                                                                            |
| -------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------- |
| `meta`                                                                                 | [operations.GetContactsV2Meta](../../models/operations/get-contacts-v2-meta.md)        | :heavy_minus_sign:                                                                     | N/A                                                                                    |
| `data`                                                                                 | [models.ContactResponseDtoV2](../../models/contact-response-dto-v2.md)[]               | :heavy_check_mark:                                                                     | N/A                                                                                    |
| `errors`                                                                               | [operations.GetContactsV2Errors](../../models/operations/get-contacts-v2-errors.md)    | :heavy_check_mark:                                                                     | N/A                                                                                    |
| `rawData`                                                                              | [operations.GetContactsV2RawData](../../models/operations/get-contacts-v2-raw-data.md) | :heavy_check_mark:                                                                     | N/A                                                                                    |