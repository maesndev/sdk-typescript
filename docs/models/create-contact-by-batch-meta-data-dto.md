# CreateContactByBatchMetaDataDto

## Example Usage

```typescript
import { CreateContactByBatchMetaDataDto } from "@maesn/typescript-sdk/models";

let value: CreateContactByBatchMetaDataDto = {
  accountNumberLength: 9374.86,
  chartOfAccount: "SKR42",
  entries: [],
  fiscalYearStartDate: "<value>",
};
```

## Fields

| Field                                                                                                                       | Type                                                                                                                        | Required                                                                                                                    | Description                                                                                                                 |
| --------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------- |
| `accountNumberLength`                                                                                                       | *number*                                                                                                                    | :heavy_check_mark:                                                                                                          | N/A                                                                                                                         |
| `chartOfAccount`                                                                                                            | [models.CreateContactByBatchMetaDataDtoChartOfAccount](../models/create-contact-by-batch-meta-data-dto-chart-of-account.md) | :heavy_check_mark:                                                                                                          | N/A                                                                                                                         |
| `entries`                                                                                                                   | [models.CreateContactRequestDtoV2](../models/create-contact-request-dto-v2.md)[]                                            | :heavy_check_mark:                                                                                                          | N/A                                                                                                                         |
| `fiscalYearStartDate`                                                                                                       | *string*                                                                                                                    | :heavy_check_mark:                                                                                                          | N/A                                                                                                                         |