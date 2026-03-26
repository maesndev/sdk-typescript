# GetProjectsResponse

## Example Usage

```typescript
import { GetProjectsResponse } from "@maesn/typescript-sdk/models/operations";

let value: GetProjectsResponse = {
  data: [
    {
      id: "<id>",
      code: "<value>",
      createdDate: "<value>",
      contactId: "<id>",
      currency: null,
      description: "serene poorly waver",
      endDate: "<value>",
      name: "<value>",
      number: "<value>",
      parentProjectId: "<id>",
      status: "CLOSED",
      startDate: null,
      updatedDate: null,
    },
  ],
  errors: null,
  rawData: {},
};
```

## Fields

| Field                                                                             | Type                                                                              | Required                                                                          | Description                                                                       |
| --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- |
| `meta`                                                                            | [operations.GetProjectsMeta](../../models/operations/get-projects-meta.md)        | :heavy_minus_sign:                                                                | N/A                                                                               |
| `data`                                                                            | [models.ProjectResponseDto](../../models/project-response-dto.md)[]               | :heavy_check_mark:                                                                | N/A                                                                               |
| `errors`                                                                          | [operations.GetProjectsErrors](../../models/operations/get-projects-errors.md)    | :heavy_check_mark:                                                                | N/A                                                                               |
| `rawData`                                                                         | [operations.GetProjectsRawData](../../models/operations/get-projects-raw-data.md) | :heavy_check_mark:                                                                | N/A                                                                               |