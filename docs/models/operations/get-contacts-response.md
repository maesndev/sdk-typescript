# GetContactsResponse

List of contacts for the authenticated end user's connected target system

## Example Usage

```typescript
import { GetContactsResponse } from "@maesn/typescript-sdk/models/operations";

let value: GetContactsResponse = {
  data: [],
  errors: null,
  rawData: {},
};
```

## Fields

| Field                                                                             | Type                                                                              | Required                                                                          | Description                                                                       |
| --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- |
| `meta`                                                                            | [operations.GetContactsMeta](../../models/operations/get-contacts-meta.md)        | :heavy_minus_sign:                                                                | N/A                                                                               |
| `data`                                                                            | [models.ContactResponseDtoV2](../../models/contact-response-dto-v2.md)[]          | :heavy_check_mark:                                                                | N/A                                                                               |
| `errors`                                                                          | [operations.GetContactsErrors](../../models/operations/get-contacts-errors.md)    | :heavy_check_mark:                                                                | N/A                                                                               |
| `rawData`                                                                         | [operations.GetContactsRawData](../../models/operations/get-contacts-raw-data.md) | :heavy_check_mark:                                                                | N/A                                                                               |