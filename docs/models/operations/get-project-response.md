# GetProjectResponse

## Example Usage

```typescript
import { GetProjectResponse } from "@maesn/typescript-sdk/models/operations";

let value: GetProjectResponse = {
  data: {
    id: "<id>",
    code: "<value>",
    createdDate: "<value>",
    contactId: "<id>",
    currency: "HKD",
    description: "drat ah thick suckle sizzling",
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

| Field                                                                           | Type                                                                            | Required                                                                        | Description                                                                     |
| ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- |
| `meta`                                                                          | [operations.GetProjectMeta](../../models/operations/get-project-meta.md)        | :heavy_minus_sign:                                                              | N/A                                                                             |
| `data`                                                                          | [models.ProjectResponseDto](../../models/project-response-dto.md)               | :heavy_check_mark:                                                              | N/A                                                                             |
| `errors`                                                                        | [operations.GetProjectErrors](../../models/operations/get-project-errors.md)    | :heavy_check_mark:                                                              | N/A                                                                             |
| `rawData`                                                                       | [operations.GetProjectRawData](../../models/operations/get-project-raw-data.md) | :heavy_check_mark:                                                              | N/A                                                                             |