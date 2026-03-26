# CreatePassThroughRequestDto

## Example Usage

```typescript
import { CreatePassThroughRequestDto } from "@maesn/typescript-sdk/models";

let value: CreatePassThroughRequestDto = {
  path: "/opt/lib",
  method: "PATCH",
};
```

## Fields

| Field                                  | Type                                   | Required                               | Description                            |
| -------------------------------------- | -------------------------------------- | -------------------------------------- | -------------------------------------- |
| `path`                                 | *string*                               | :heavy_check_mark:                     | N/A                                    |
| `method`                               | [models.Method](../models/method.md)   | :heavy_check_mark:                     | N/A                                    |
| `headers`                              | [models.Headers](../models/headers.md) | :heavy_minus_sign:                     | N/A                                    |
| `body`                                 | [models.Body](../models/body.md)       | :heavy_minus_sign:                     | N/A                                    |
| `query`                                | [models.Query](../models/query.md)     | :heavy_minus_sign:                     | N/A                                    |