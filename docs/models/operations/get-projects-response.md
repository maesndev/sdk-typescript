# GetProjectsResponse

## Example Usage

```typescript
import { GetProjectsResponse } from "maesn/models/operations";

let value: GetProjectsResponse = {
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
  data: [
    {
      id: "<id>",
      code: "<value>",
      createdDate: "<value>",
      contactId: "<id>",
      currency: "GIP",
      description:
        "evenly afford cheese juvenile anxiously dowse wretched brood aw",
      endDate: "<value>",
      name: "<value>",
      number: "<value>",
      parentProjectId: "<id>",
      status: "CLOSED",
      startDate: "<value>",
      updatedDate: "<value>",
    },
  ],
  errors: {},
  rawData: {},
};
```

## Fields

| Field                                                                             | Type                                                                              | Required                                                                          | Description                                                                       |
| --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- |
| `meta`                                                                            | [models.MetaResponse](../../models/meta-response.md)                              | :heavy_check_mark:                                                                | N/A                                                                               |
| `data`                                                                            | [models.ProjectResponseDto](../../models/project-response-dto.md)[]               | :heavy_check_mark:                                                                | N/A                                                                               |
| `errors`                                                                          | [operations.GetProjectsErrors](../../models/operations/get-projects-errors.md)    | :heavy_check_mark:                                                                | N/A                                                                               |
| `rawData`                                                                         | [operations.GetProjectsRawData](../../models/operations/get-projects-raw-data.md) | :heavy_check_mark:                                                                | N/A                                                                               |