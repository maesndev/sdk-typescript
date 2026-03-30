# CallbackRequest

## Example Usage

```typescript
import { CallbackRequest } from "@maesn/typescript-sdk/models/operations";

let value: CallbackRequest = {
  targetSystem: "<value>",
  state: "West Virginia",
};
```

## Fields

| Field                                                                                            | Type                                                                                             | Required                                                                                         | Description                                                                                      |
| ------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------ |
| `targetSystem`                                                                                   | *string*                                                                                         | :heavy_check_mark:                                                                               | N/A                                                                                              |
| `state`                                                                                          | *string*                                                                                         | :heavy_check_mark:                                                                               | OAuth state parameter returned by the target system, encoding tenant and user context            |
| `code`                                                                                           | *string*                                                                                         | :heavy_minus_sign:                                                                               | Authorization code returned by the target system after successful OAuth consent                  |
| `realmId`                                                                                        | *string*                                                                                         | :heavy_minus_sign:                                                                               | Realm ID returned by QuickBooks Online after OAuth consent                                       |
| `token`                                                                                          | *string*                                                                                         | :heavy_minus_sign:                                                                               | Access token returned directly by some target systems that do not use an authorization code flow |