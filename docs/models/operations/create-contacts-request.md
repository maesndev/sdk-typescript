# CreateContactsRequest

## Example Usage

```typescript
import { CreateContactsRequest } from "@maesn/typescript-sdk/models/operations";

let value: CreateContactsRequest = {
  body: {
    accountNumberLength: 1615.04,
    chartOfAccount: "SKR42",
    entries: [],
    fiscalYearStartDate: "<value>",
  },
};
```

## Fields

| Field                                                                                           | Type                                                                                            | Required                                                                                        | Description                                                                                     |
| ----------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------- |
| `companyId`                                                                                     | *string*                                                                                        | :heavy_minus_sign:                                                                              | N/A                                                                                             |
| `body`                                                                                          | [models.CreateContactByBatchMetaDataDto](../../models/create-contact-by-batch-meta-data-dto.md) | :heavy_check_mark:                                                                              | N/A                                                                                             |