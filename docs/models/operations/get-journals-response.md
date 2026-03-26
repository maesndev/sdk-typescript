# GetJournalsResponse

## Example Usage

```typescript
import { GetJournalsResponse } from "@maesn/typescript-sdk/models/operations";

let value: GetJournalsResponse = {
  data: [],
  errors: {},
  rawData: null,
};
```

## Fields

| Field                                                                             | Type                                                                              | Required                                                                          | Description                                                                       |
| --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- |
| `meta`                                                                            | [operations.GetJournalsMeta](../../models/operations/get-journals-meta.md)        | :heavy_minus_sign:                                                                | N/A                                                                               |
| `data`                                                                            | [models.JournalResponseDto](../../models/journal-response-dto.md)[]               | :heavy_check_mark:                                                                | N/A                                                                               |
| `errors`                                                                          | [operations.GetJournalsErrors](../../models/operations/get-journals-errors.md)    | :heavy_check_mark:                                                                | N/A                                                                               |
| `rawData`                                                                         | [operations.GetJournalsRawData](../../models/operations/get-journals-raw-data.md) | :heavy_check_mark:                                                                | N/A                                                                               |