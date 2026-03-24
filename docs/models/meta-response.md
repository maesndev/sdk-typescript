# MetaResponse

## Example Usage

```typescript
import { MetaResponse } from "maesn/models";

let value: MetaResponse = {
  warnings: [
    "<value 1>",
  ],
  pagination: {
    total: 3438.77,
    perPage: 5109.63,
    currentPage: 2626.79,
    totalPages: 3561.84,
  },
};
```

## Fields

| Field                                                         | Type                                                          | Required                                                      | Description                                                   |
| ------------------------------------------------------------- | ------------------------------------------------------------- | ------------------------------------------------------------- | ------------------------------------------------------------- |
| `warnings`                                                    | *string*[]                                                    | :heavy_check_mark:                                            | N/A                                                           |
| `pagination`                                                  | [models.PaginationResponse](../models/pagination-response.md) | :heavy_check_mark:                                            | N/A                                                           |