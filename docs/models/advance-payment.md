# AdvancePayment

## Example Usage

```typescript
import { AdvancePayment } from "@maesn/typescript-sdk/models";

let value: AdvancePayment = {
  orderNumber: null,
  type: "FINAL_INVOICE",
};
```

## Fields

| Field                                                                              | Type                                                                               | Required                                                                           | Description                                                                        |
| ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- |
| `orderNumber`                                                                      | *string*                                                                           | :heavy_check_mark:                                                                 | N/A                                                                                |
| `type`                                                                             | [models.JournalEntryResponseDtoType](../models/journal-entry-response-dto-type.md) | :heavy_check_mark:                                                                 | N/A                                                                                |