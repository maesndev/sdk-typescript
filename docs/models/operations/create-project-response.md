# CreateProjectResponse

## Example Usage

```typescript
import { CreateProjectResponse } from "maesn/models/operations";

let value: CreateProjectResponse = {
  meta: {
    warnings: [
      "<value 1>",
      "<value 2>",
    ],
    pagination: {
      total: 3438.77,
      perPage: 5109.63,
      currentPage: 2626.79,
      totalPages: 3561.84,
    },
  },
  data: {
    id: "<id>",
    code: "<value>",
    createdDate: "<value>",
    contactId: "<id>",
    currency: "DOP",
    description:
      "apud spectate regularly clumsy incomplete intelligent spherical nor",
    endDate: "<value>",
    name: "<value>",
    number: "<value>",
    parentProjectId: "<id>",
    status: "ACTIVE",
    startDate: "<value>",
    updatedDate: "<value>",
  },
  errors: {},
  rawData: {},
};
```

## Fields

| Field                                                                                 | Type                                                                                  | Required                                                                              | Description                                                                           |
| ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- |
| `meta`                                                                                | [models.MetaResponse](../../models/meta-response.md)                                  | :heavy_check_mark:                                                                    | N/A                                                                                   |
| `data`                                                                                | [models.ProjectResponseDto](../../models/project-response-dto.md)                     | :heavy_check_mark:                                                                    | N/A                                                                                   |
| `errors`                                                                              | [operations.CreateProjectErrors](../../models/operations/create-project-errors.md)    | :heavy_check_mark:                                                                    | N/A                                                                                   |
| `rawData`                                                                             | [operations.CreateProjectRawData](../../models/operations/create-project-raw-data.md) | :heavy_check_mark:                                                                    | N/A                                                                                   |