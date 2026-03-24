# CreateProjectRequest

## Example Usage

```typescript
import { CreateProjectRequest } from "maesn/models/operations";

let value: CreateProjectRequest = {
  body: {
    code: "<value>",
    contactId: "<id>",
    currency: "YER",
    description: "coop worthwhile huzzah spotless",
    endDate: "<value>",
    name: "<value>",
    number: "<value>",
    parentProjectId: "<id>",
    status: "ACTIVE",
    startDate: "<value>",
  },
};
```

## Fields

| Field                                                                        | Type                                                                         | Required                                                                     | Description                                                                  |
| ---------------------------------------------------------------------------- | ---------------------------------------------------------------------------- | ---------------------------------------------------------------------------- | ---------------------------------------------------------------------------- |
| `environmentName`                                                            | *string*                                                                     | :heavy_minus_sign:                                                           | N/A                                                                          |
| `companyId`                                                                  | *string*                                                                     | :heavy_minus_sign:                                                           | N/A                                                                          |
| `xApiKey`                                                                    | *string*                                                                     | :heavy_minus_sign:                                                           | API key                                                                      |
| `xAccountKey`                                                                | *string*                                                                     | :heavy_minus_sign:                                                           | Account key                                                                  |
| `body`                                                                       | [models.CreateProjectRequestDto](../../models/create-project-request-dto.md) | :heavy_check_mark:                                                           | N/A                                                                          |