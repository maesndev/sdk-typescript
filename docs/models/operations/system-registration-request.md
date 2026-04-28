# SystemRegistrationRequest

## Example Usage

```typescript
import { SystemRegistrationRequest } from "@maesn/typescript-sdk/models/operations";

let value: SystemRegistrationRequest = {
  body: {
    targetSystem: "<value>",
    clientId: "<id>",
    clientSecret: "<value>",
    customValues: [
      {
        key: "<key>",
        value: "<value>",
      },
    ],
  },
};
```

## Fields

| Field                                                                   | Type                                                                    | Required                                                                | Description                                                             |
| ----------------------------------------------------------------------- | ----------------------------------------------------------------------- | ----------------------------------------------------------------------- | ----------------------------------------------------------------------- |
| `apiKey`                                                                | *string*                                                                | :heavy_minus_sign:                                                      | API key                                                                 |
| `accountKey`                                                            | *string*                                                                | :heavy_minus_sign:                                                      | Account key                                                             |
| `body`                                                                  | [models.SystemRegistrationDto](../../models/system-registration-dto.md) | :heavy_check_mark:                                                      | N/A                                                                     |