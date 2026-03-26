# GetBookingProposalDocumentResponse

## Example Usage

```typescript
import { GetBookingProposalDocumentResponse } from "@maesn/typescript-sdk/models/operations";

let value: GetBookingProposalDocumentResponse = {
  data: {
    id: "<id>",
    base64Encoded: true,
    content: "<value>",
    contentType: "<value>",
    fileName: "example.file",
  },
  errors: {},
  rawData: null,
};
```

## Fields

| Field                                                                                                             | Type                                                                                                              | Required                                                                                                          | Description                                                                                                       |
| ----------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------- |
| `meta`                                                                                                            | [operations.GetBookingProposalDocumentMeta](../../models/operations/get-booking-proposal-document-meta.md)        | :heavy_minus_sign:                                                                                                | N/A                                                                                                               |
| `data`                                                                                                            | [models.DocumentResponseDto](../../models/document-response-dto.md)                                               | :heavy_check_mark:                                                                                                | N/A                                                                                                               |
| `errors`                                                                                                          | [operations.GetBookingProposalDocumentErrors](../../models/operations/get-booking-proposal-document-errors.md)    | :heavy_check_mark:                                                                                                | N/A                                                                                                               |
| `rawData`                                                                                                         | [operations.GetBookingProposalDocumentRawData](../../models/operations/get-booking-proposal-document-raw-data.md) | :heavy_check_mark:                                                                                                | N/A                                                                                                               |