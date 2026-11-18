# ValidateConnectionResponse

Validates the connection for the authenticated end user

## Example Usage

```typescript
import { ValidateConnectionResponse } from "@maesn/typescript-sdk/models/operations";

let value: ValidateConnectionResponse = {
  data: {
    valid: false,
    targetSystem: "<value>",
  },
  errors: {},
  rawData: {},
};
```

## Fields

| Field                                                                                           | Type                                                                                            | Required                                                                                        | Description                                                                                     |
| ----------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------- |
| `meta`                                                                                          | [operations.ValidateConnectionMeta](../../models/operations/validate-connection-meta.md)        | :heavy_minus_sign:                                                                              | N/A                                                                                             |
| `data`                                                                                          | [models.ConnectionValidationResponseDto](../../models/connection-validation-response-dto.md)    | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `errors`                                                                                        | [operations.ValidateConnectionErrors](../../models/operations/validate-connection-errors.md)    | :heavy_check_mark:                                                                              | N/A                                                                                             |
| `rawData`                                                                                       | [operations.ValidateConnectionRawData](../../models/operations/validate-connection-raw-data.md) | :heavy_check_mark:                                                                              | N/A                                                                                             |