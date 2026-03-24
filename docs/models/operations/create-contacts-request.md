# CreateContactsRequest

## Example Usage

```typescript
import { CreateContactsRequest } from "maesn/models/operations";

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
| `xApiKey`                                                                                       | *string*                                                                                        | :heavy_minus_sign:                                                                              | API key                                                                                         |
| `xAccountKey`                                                                                   | *string*                                                                                        | :heavy_minus_sign:                                                                              | Account key                                                                                     |
| `body`                                                                                          | [models.CreateContactByBatchMetaDataDto](../../models/create-contact-by-batch-meta-data-dto.md) | :heavy_check_mark:                                                                              | N/A                                                                                             |