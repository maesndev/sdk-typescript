# CreatePassThroughRequestDto

## Example Usage

```typescript
import { CreatePassThroughRequestDto } from "maesn/models";

let value: CreatePassThroughRequestDto = {
  path: "/opt/lib",
  method: "PATCH",
  headers: {},
  body: {},
  query: {},
};
```

## Fields

| Field                                  | Type                                   | Required                               | Description                            |
| -------------------------------------- | -------------------------------------- | -------------------------------------- | -------------------------------------- |
| `path`                                 | *string*                               | :heavy_check_mark:                     | N/A                                    |
| `method`                               | [models.Method](../models/method.md)   | :heavy_check_mark:                     | N/A                                    |
| `headers`                              | [models.Headers](../models/headers.md) | :heavy_check_mark:                     | N/A                                    |
| `body`                                 | [models.Body](../models/body.md)       | :heavy_check_mark:                     | N/A                                    |
| `query`                                | [models.Query](../models/query.md)     | :heavy_check_mark:                     | N/A                                    |