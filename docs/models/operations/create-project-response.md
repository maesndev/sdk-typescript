# CreateProjectResponse

Project created successfully. Returns 202 with taskId if processed asynchronously.

## Example Usage

```typescript
import { CreateProjectResponse } from "@maesn/typescript-sdk/models/operations";

let value: CreateProjectResponse = {
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
  rawData: null,
};
```

## Fields

| Field                                                                                 | Type                                                                                  | Required                                                                              | Description                                                                           |
| ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- |
| `meta`                                                                                | [operations.CreateProjectMeta](../../models/operations/create-project-meta.md)        | :heavy_minus_sign:                                                                    | N/A                                                                                   |
| `data`                                                                                | [models.ProjectResponseDto](../../models/project-response-dto.md)                     | :heavy_check_mark:                                                                    | N/A                                                                                   |
| `errors`                                                                              | [operations.CreateProjectErrors](../../models/operations/create-project-errors.md)    | :heavy_check_mark:                                                                    | N/A                                                                                   |
| `rawData`                                                                             | [operations.CreateProjectRawData](../../models/operations/create-project-raw-data.md) | :heavy_check_mark:                                                                    | N/A                                                                                   |