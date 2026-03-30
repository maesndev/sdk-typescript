# CreateContactsV1Request

## Example Usage

```typescript
import { CreateContactsV1Request } from "@maesn/typescript-sdk/models/operations";

let value: CreateContactsV1Request = {
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
| `companyId`                                                                                     | *string*                                                                                        | :heavy_minus_sign:                                                                              | ID of the company (required for multi-company target systems)                                   |
| `body`                                                                                          | [models.CreateContactByBatchMetaDataDto](../../models/create-contact-by-batch-meta-data-dto.md) | :heavy_check_mark:                                                                              | N/A                                                                                             |