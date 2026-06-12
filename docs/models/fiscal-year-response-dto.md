# FiscalYearResponseDto

## Example Usage

```typescript
import { FiscalYearResponseDto } from "@maesn/typescript-sdk/models";

let value: FiscalYearResponseDto = {
  id: "<id>",
  accountNumberLength: 3809.97,
  availableLedgers: [],
  chartOfAccount: "SKR03",
  createdDate: "<value>",
  description: "pluck split bruised whose ick meh how sometimes",
  endDate: "<value>",
  startDate: "<value>",
  status: "CLOSED",
  updatedDate: "<value>",
};
```

## Fields

| Field                                                                                                | Type                                                                                                 | Required                                                                                             | Description                                                                                          |
| ---------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------- |
| `id`                                                                                                 | *string*                                                                                             | :heavy_check_mark:                                                                                   | N/A                                                                                                  |
| `accountNumberLength`                                                                                | *number*                                                                                             | :heavy_check_mark:                                                                                   | N/A                                                                                                  |
| `availableLedgers`                                                                                   | [models.AvailableLedger](../models/available-ledger.md)[]                                            | :heavy_check_mark:                                                                                   | N/A                                                                                                  |
| `chartOfAccount`                                                                                     | [models.FiscalYearResponseDtoChartOfAccount](../models/fiscal-year-response-dto-chart-of-account.md) | :heavy_check_mark:                                                                                   | N/A                                                                                                  |
| `createdDate`                                                                                        | *string*                                                                                             | :heavy_check_mark:                                                                                   | N/A                                                                                                  |
| `description`                                                                                        | *string*                                                                                             | :heavy_check_mark:                                                                                   | N/A                                                                                                  |
| `endDate`                                                                                            | *string*                                                                                             | :heavy_check_mark:                                                                                   | N/A                                                                                                  |
| `startDate`                                                                                          | *string*                                                                                             | :heavy_check_mark:                                                                                   | N/A                                                                                                  |
| `status`                                                                                             | [models.FiscalYearResponseDtoStatus](../models/fiscal-year-response-dto-status.md)                   | :heavy_check_mark:                                                                                   | N/A                                                                                                  |
| `updatedDate`                                                                                        | *string*                                                                                             | :heavy_check_mark:                                                                                   | N/A                                                                                                  |