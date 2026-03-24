# FiscalYearResponseDto

## Example Usage

```typescript
import { FiscalYearResponseDto } from "maesn/models";

let value: FiscalYearResponseDto = {
  id: "<id>",
  accountNumberLength: 3809.97,
  chartOfAccount: "SKR51",
  createdDate: "<value>",
  description: "though gadzooks spiffy",
  endDate: "<value>",
  startDate: "<value>",
  status: "OPEN",
  updatedDate: "<value>",
};
```

## Fields

| Field                                                                                                | Type                                                                                                 | Required                                                                                             | Description                                                                                          |
| ---------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------- |
| `id`                                                                                                 | *string*                                                                                             | :heavy_check_mark:                                                                                   | N/A                                                                                                  |
| `accountNumberLength`                                                                                | *number*                                                                                             | :heavy_check_mark:                                                                                   | N/A                                                                                                  |
| `chartOfAccount`                                                                                     | [models.FiscalYearResponseDtoChartOfAccount](../models/fiscal-year-response-dto-chart-of-account.md) | :heavy_check_mark:                                                                                   | N/A                                                                                                  |
| `createdDate`                                                                                        | *string*                                                                                             | :heavy_check_mark:                                                                                   | N/A                                                                                                  |
| `description`                                                                                        | *string*                                                                                             | :heavy_check_mark:                                                                                   | N/A                                                                                                  |
| `endDate`                                                                                            | *string*                                                                                             | :heavy_check_mark:                                                                                   | N/A                                                                                                  |
| `startDate`                                                                                          | *string*                                                                                             | :heavy_check_mark:                                                                                   | N/A                                                                                                  |
| `status`                                                                                             | [models.FiscalYearResponseDtoStatus](../models/fiscal-year-response-dto-status.md)                   | :heavy_check_mark:                                                                                   | N/A                                                                                                  |
| `updatedDate`                                                                                        | *string*                                                                                             | :heavy_check_mark:                                                                                   | N/A                                                                                                  |