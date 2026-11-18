# ConnectionValidationResponseDto

## Example Usage

```typescript
import { ConnectionValidationResponseDto } from "@maesn/typescript-sdk/models";

let value: ConnectionValidationResponseDto = {
  valid: false,
  targetSystem: "<value>",
};
```

## Fields

| Field                                                             | Type                                                              | Required                                                          | Description                                                       |
| ----------------------------------------------------------------- | ----------------------------------------------------------------- | ----------------------------------------------------------------- | ----------------------------------------------------------------- |
| `valid`                                                           | *boolean*                                                         | :heavy_check_mark:                                                | Whether the connection is valid and can be used to make API calls |
| `targetSystem`                                                    | *string*                                                          | :heavy_check_mark:                                                | The target system identifier                                      |