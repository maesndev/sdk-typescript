# CreateProjectRequest

## Example Usage

```typescript
import { CreateProjectRequest } from "@maesn/typescript-sdk/models/operations";

let value: CreateProjectRequest = {
  body: {},
};
```

## Fields

| Field                                                                              | Type                                                                               | Required                                                                           | Description                                                                        |
| ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- |
| `environmentName`                                                                  | *string*                                                                           | :heavy_minus_sign:                                                                 | Environment name (required for multi-environment systems such as Business Central) |
| `companyId`                                                                        | *string*                                                                           | :heavy_minus_sign:                                                                 | ID of the company (required for multi-company target systems)                      |
| `apiKey`                                                                           | *string*                                                                           | :heavy_minus_sign:                                                                 | API key                                                                            |
| `accountKey`                                                                       | *string*                                                                           | :heavy_minus_sign:                                                                 | Account key                                                                        |
| `body`                                                                             | [models.CreateProjectRequestDto](../../models/create-project-request-dto.md)       | :heavy_check_mark:                                                                 | N/A                                                                                |