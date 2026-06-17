# CreateCreditNoteRequest

## Example Usage

```typescript
import { CreateCreditNoteRequest } from "@maesn/typescript-sdk/models/operations";

let value: CreateCreditNoteRequest = {
  body: {
    creditNoteDate: "<value>",
    creditNoteLines: [],
  },
};
```

## Fields

| Field                                                                               | Type                                                                                | Required                                                                            | Description                                                                         |
| ----------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------- |
| `apiKey`                                                                            | *string*                                                                            | :heavy_minus_sign:                                                                  | API key                                                                             |
| `accountKey`                                                                        | *string*                                                                            | :heavy_minus_sign:                                                                  | Account key                                                                         |
| `body`                                                                              | [models.CreateCreditNoteRequestDto](../../models/create-credit-note-request-dto.md) | :heavy_check_mark:                                                                  | N/A                                                                                 |