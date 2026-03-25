# CompanyResponseDto

## Example Usage

```typescript
import { CompanyResponseDto } from "maesn/models";

let value: CompanyResponseDto = {
  id: "<id>",
  name: "<value>",
  environmentId: "<id>",
  clientNumber: 8632.65,
  consultantNumber: 1584.86,
  subscription: {
    id: "<id>",
    name: "<value>",
    status: "<value>",
    active: false,
  },
};
```

## Fields

| Field                                            | Type                                             | Required                                         | Description                                      |
| ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------ |
| `id`                                             | *string*                                         | :heavy_check_mark:                               | N/A                                              |
| `name`                                           | *string*                                         | :heavy_check_mark:                               | N/A                                              |
| `environmentId`                                  | *string*                                         | :heavy_check_mark:                               | N/A                                              |
| `clientNumber`                                   | *number*                                         | :heavy_check_mark:                               | N/A                                              |
| `consultantNumber`                               | *number*                                         | :heavy_check_mark:                               | N/A                                              |
| `subscription`                                   | [models.Subscription](../models/subscription.md) | :heavy_check_mark:                               | N/A                                              |