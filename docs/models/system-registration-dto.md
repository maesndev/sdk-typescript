# SystemRegistrationDto

## Example Usage

```typescript
import { SystemRegistrationDto } from "@maesn/typescript-sdk/models";

let value: SystemRegistrationDto = {
  targetSystem: "<value>",
  clientId: "<id>",
  clientSecret: "<value>",
  customValues: [
    {
      key: "<key>",
      value: "<value>",
    },
  ],
};
```

## Fields

| Field                                               | Type                                                | Required                                            | Description                                         |
| --------------------------------------------------- | --------------------------------------------------- | --------------------------------------------------- | --------------------------------------------------- |
| `targetSystem`                                      | *string*                                            | :heavy_check_mark:                                  | N/A                                                 |
| `clientId`                                          | *string*                                            | :heavy_check_mark:                                  | N/A                                                 |
| `clientSecret`                                      | *string*                                            | :heavy_check_mark:                                  | N/A                                                 |
| `customValues`                                      | [models.CustomValues](../models/custom-values.md)[] | :heavy_check_mark:                                  | N/A                                                 |