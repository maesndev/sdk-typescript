# CreateEndUserAccountRequest

## Example Usage

```typescript
import { CreateEndUserAccountRequest } from "@maesn/typescript-sdk/models/operations";

let value: CreateEndUserAccountRequest = {
  targetSystem: "<value>",
  body: {
    apiKey: "<value>",
    baseUrl: "https://minor-community.name/",
    clientName: "<value>",
    clientSecret: "<value>",
    database: "<value>",
    mandant: "<value>",
    password: "cTG3VYatE1yWypi",
    tenantId: "<id>",
    url: "https://clumsy-community.com/",
    username: "Roscoe.Dietrich",
  },
};
```

## Fields

| Field                                                                         | Type                                                                          | Required                                                                      | Description                                                                   |
| ----------------------------------------------------------------------------- | ----------------------------------------------------------------------------- | ----------------------------------------------------------------------------- | ----------------------------------------------------------------------------- |
| `targetSystem`                                                                | *string*                                                                      | :heavy_check_mark:                                                            | N/A                                                                           |
| `apiKey`                                                                      | *string*                                                                      | :heavy_minus_sign:                                                            | API key                                                                       |
| `accountKey`                                                                  | *string*                                                                      | :heavy_minus_sign:                                                            | Account key                                                                   |
| `body`                                                                        | [models.CreateEndUserRequestDto](../../models/create-end-user-request-dto.md) | :heavy_check_mark:                                                            | N/A                                                                           |