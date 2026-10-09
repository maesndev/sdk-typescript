# CreateBookingProposalAttachmentResponse

Booking proposal attachment uploaded successfully

## Example Usage

```typescript
import { CreateBookingProposalAttachmentResponse } from "@maesn/typescript-sdk/models/operations";

let value: CreateBookingProposalAttachmentResponse = {
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

| Field                                                                                                                       | Type                                                                                                                        | Required                                                                                                                    | Description                                                                                                                 |
| --------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------- |
| `meta`                                                                                                                      | [operations.CreateBookingProposalAttachmentMeta](../../models/operations/create-booking-proposal-attachment-meta.md)        | :heavy_minus_sign:                                                                                                          | N/A                                                                                                                         |
| `data`                                                                                                                      | [models.DocumentResponseDto](../../models/document-response-dto.md)                                                         | :heavy_check_mark:                                                                                                          | N/A                                                                                                                         |
| `errors`                                                                                                                    | [operations.CreateBookingProposalAttachmentErrors](../../models/operations/create-booking-proposal-attachment-errors.md)    | :heavy_check_mark:                                                                                                          | N/A                                                                                                                         |
| `rawData`                                                                                                                   | [operations.CreateBookingProposalAttachmentRawData](../../models/operations/create-booking-proposal-attachment-raw-data.md) | :heavy_check_mark:                                                                                                          | N/A                                                                                                                         |