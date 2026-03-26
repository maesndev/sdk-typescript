# ServiceUnavailableError

The Health Check is not successful

## Example Usage

```typescript
import { ServiceUnavailableError } from "@maesn/typescript-sdk/models/errors";

// No examples available for this model
```

## Fields

| Field                                                                                             | Type                                                                                              | Required                                                                                          | Description                                                                                       | Example                                                                                           |
| ------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------- |
| `status`                                                                                          | *string*                                                                                          | :heavy_minus_sign:                                                                                | N/A                                                                                               | error                                                                                             |
| `info`                                                                                            | Record<string, [operations.Info](../../models/operations/info.md)>                                | :heavy_minus_sign:                                                                                | N/A                                                                                               | {<br/>"database": {<br/>"status": "up"<br/>}<br/>}                                                |
| `error`                                                                                           | Record<string, [operations.ErrorT](../../models/operations/error-t.md)>                           | :heavy_minus_sign:                                                                                | N/A                                                                                               | {<br/>"redis": {<br/>"status": "down",<br/>"message": "Could not connect"<br/>}<br/>}             |
| `details`                                                                                         | Record<string, [operations.Details](../../models/operations/details.md)>                          | :heavy_minus_sign:                                                                                | N/A                                                                                               | {<br/>"database": {<br/>"status": "up"<br/>},<br/>"redis": {<br/>"status": "down",<br/>"message": "Could not connect"<br/>}<br/>} |