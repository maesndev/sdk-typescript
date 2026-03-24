# ProjectResponseDto

## Example Usage

```typescript
import { ProjectResponseDto } from "maesn/models";

let value: ProjectResponseDto = {
  id: "<id>",
  code: "<value>",
  createdDate: "<value>",
  contactId: "<id>",
  currency: "KWD",
  description: "shadowy denitrify ew",
  endDate: "<value>",
  name: "<value>",
  number: "<value>",
  parentProjectId: "<id>",
  status: "ACTIVE",
  startDate: "<value>",
  updatedDate: "<value>",
};
```

## Fields

| Field                                                                           | Type                                                                            | Required                                                                        | Description                                                                     |
| ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- |
| `id`                                                                            | *string*                                                                        | :heavy_check_mark:                                                              | N/A                                                                             |
| `code`                                                                          | *string*                                                                        | :heavy_check_mark:                                                              | N/A                                                                             |
| `createdDate`                                                                   | *string*                                                                        | :heavy_check_mark:                                                              | N/A                                                                             |
| `contactId`                                                                     | *string*                                                                        | :heavy_check_mark:                                                              | N/A                                                                             |
| `currency`                                                                      | [models.ProjectResponseDtoCurrency](../models/project-response-dto-currency.md) | :heavy_check_mark:                                                              | N/A                                                                             |
| `description`                                                                   | *string*                                                                        | :heavy_check_mark:                                                              | N/A                                                                             |
| `endDate`                                                                       | *string*                                                                        | :heavy_check_mark:                                                              | N/A                                                                             |
| `name`                                                                          | *string*                                                                        | :heavy_check_mark:                                                              | N/A                                                                             |
| `number`                                                                        | *string*                                                                        | :heavy_check_mark:                                                              | N/A                                                                             |
| `parentProjectId`                                                               | *string*                                                                        | :heavy_check_mark:                                                              | N/A                                                                             |
| `status`                                                                        | [models.ProjectResponseDtoStatus](../models/project-response-dto-status.md)     | :heavy_check_mark:                                                              | N/A                                                                             |
| `startDate`                                                                     | *string*                                                                        | :heavy_check_mark:                                                              | N/A                                                                             |
| `updatedDate`                                                                   | *string*                                                                        | :heavy_check_mark:                                                              | N/A                                                                             |