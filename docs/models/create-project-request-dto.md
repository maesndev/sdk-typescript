# CreateProjectRequestDto

## Example Usage

```typescript
import { CreateProjectRequestDto } from "maesn/models";

let value: CreateProjectRequestDto = {
  code: "<value>",
  contactId: "<id>",
  currency: "HNL",
  description: "curse ack train",
  endDate: "<value>",
  name: "<value>",
  number: "<value>",
  parentProjectId: "<id>",
  status: "ACTIVE",
  startDate: "<value>",
};
```

## Fields

| Field                                                                                      | Type                                                                                       | Required                                                                                   | Description                                                                                |
| ------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------ |
| `code`                                                                                     | *string*                                                                                   | :heavy_check_mark:                                                                         | N/A                                                                                        |
| `contactId`                                                                                | *string*                                                                                   | :heavy_check_mark:                                                                         | N/A                                                                                        |
| `currency`                                                                                 | [models.CreateProjectRequestDtoCurrency](../models/create-project-request-dto-currency.md) | :heavy_check_mark:                                                                         | N/A                                                                                        |
| `description`                                                                              | *string*                                                                                   | :heavy_check_mark:                                                                         | N/A                                                                                        |
| `endDate`                                                                                  | *string*                                                                                   | :heavy_check_mark:                                                                         | N/A                                                                                        |
| `name`                                                                                     | *string*                                                                                   | :heavy_check_mark:                                                                         | N/A                                                                                        |
| `number`                                                                                   | *string*                                                                                   | :heavy_check_mark:                                                                         | N/A                                                                                        |
| `parentProjectId`                                                                          | *string*                                                                                   | :heavy_check_mark:                                                                         | N/A                                                                                        |
| `status`                                                                                   | [models.CreateProjectRequestDtoStatus](../models/create-project-request-dto-status.md)     | :heavy_check_mark:                                                                         | N/A                                                                                        |
| `startDate`                                                                                | *string*                                                                                   | :heavy_check_mark:                                                                         | N/A                                                                                        |