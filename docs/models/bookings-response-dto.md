# BookingsResponseDto

## Example Usage

```typescript
import { BookingsResponseDto } from "maesn/models";

let value: BookingsResponseDto = {
  id: "<id>",
  accountNumberLength: 7323.86,
  chartOfAccount: "SKR03",
  createdDate: "<value>",
  entries: [],
  fiscalYearStartDate: "<value>",
  taskId: "<id>",
};
```

## Fields

| Field                                                                                           | Type                                                                                            | Required                                                                                        | Description                                                                                     |
| ----------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------- |
| `id`                                                                                            | *string*                                                                                        | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `accountNumberLength`                                                                           | *number*                                                                                        | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `chartOfAccount`                                                                                | [models.BookingsResponseDtoChartOfAccount](../models/bookings-response-dto-chart-of-account.md) | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `createdDate`                                                                                   | *string*                                                                                        | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `entries`                                                                                       | [models.BookingEntryResponseDto](../models/booking-entry-response-dto.md)[]                     | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `fiscalYearStartDate`                                                                           | *string*                                                                                        | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `taskId`                                                                                        | *string*                                                                                        | :heavy_check_mark:                                                                              | N/A                                                                                             |