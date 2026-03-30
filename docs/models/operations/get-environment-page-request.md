# GetEnvironmentPageRequest

## Example Usage

```typescript
import { GetEnvironmentPageRequest } from "@maesn/typescript-sdk/models/operations";

let value: GetEnvironmentPageRequest = {
  state: "Illinois",
  targetSystem: "<value>",
};
```

## Fields

| Field                                                                                    | Type                                                                                     | Required                                                                                 | Description                                                                              |
| ---------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------- |
| `state`                                                                                  | *string*                                                                                 | :heavy_check_mark:                                                                       | Encoded state value containing tenant and user context, returned from the OAuth redirect |
| `targetSystem`                                                                           | *string*                                                                                 | :heavy_check_mark:                                                                       | Identifier of the target system (e.g. exact, sevdesk, xero)                              |