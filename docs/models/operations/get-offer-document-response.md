# GetOfferDocumentResponse

Document attached to the offer matching the provided ID

## Example Usage

```typescript
import { GetOfferDocumentResponse } from "@maesn/typescript-sdk/models/operations";

let value: GetOfferDocumentResponse = {
  data: {
    id: "<id>",
    base64Encoded: true,
    content: "<value>",
    contentType: "<value>",
    fileName: "example.file",
  },
  errors: {},
  rawData: {},
};
```

## Fields

| Field                                                                                        | Type                                                                                         | Required                                                                                     | Description                                                                                  |
| -------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------- |
| `meta`                                                                                       | [operations.GetOfferDocumentMeta](../../models/operations/get-offer-document-meta.md)        | :heavy_minus_sign:                                                                           | N/A                                                                                          |
| `data`                                                                                       | [models.DocumentResponseDto](../../models/document-response-dto.md)                          | :heavy_check_mark:                                                                           | N/A                                                                                          |
| `errors`                                                                                     | [operations.GetOfferDocumentErrors](../../models/operations/get-offer-document-errors.md)    | :heavy_check_mark:                                                                           | N/A                                                                                          |
| `rawData`                                                                                    | [operations.GetOfferDocumentRawData](../../models/operations/get-offer-document-raw-data.md) | :heavy_check_mark:                                                                           | N/A                                                                                          |