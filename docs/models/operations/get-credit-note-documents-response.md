# GetCreditNoteDocumentsResponse

Documents associated with the specified credit note

## Example Usage

```typescript
import { GetCreditNoteDocumentsResponse } from "@maesn/typescript-sdk/models/operations";

let value: GetCreditNoteDocumentsResponse = {
  data: [],
  errors: {},
  rawData: {},
};
```

## Fields

| Field                                                                                                     | Type                                                                                                      | Required                                                                                                  | Description                                                                                               |
| --------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------- |
| `meta`                                                                                                    | [operations.GetCreditNoteDocumentsMeta](../../models/operations/get-credit-note-documents-meta.md)        | :heavy_minus_sign:                                                                                        | N/A                                                                                                       |
| `data`                                                                                                    | [models.DocumentResponseDto](../../models/document-response-dto.md)[]                                     | :heavy_check_mark:                                                                                        | N/A                                                                                                       |
| `errors`                                                                                                  | [operations.GetCreditNoteDocumentsErrors](../../models/operations/get-credit-note-documents-errors.md)    | :heavy_check_mark:                                                                                        | N/A                                                                                                       |
| `rawData`                                                                                                 | [operations.GetCreditNoteDocumentsRawData](../../models/operations/get-credit-note-documents-raw-data.md) | :heavy_check_mark:                                                                                        | N/A                                                                                                       |