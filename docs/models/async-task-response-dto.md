# AsyncTaskResponseDto

## Example Usage

```typescript
import { AsyncTaskResponseDto } from "@maesn/typescript-sdk/models";

let value: AsyncTaskResponseDto = {
  information: [
    {
      filename: "example.file",
      message: "<value>",
      timestamp: "<value>",
      type: null,
    },
  ],
  responseData: {},
  status: null,
};
```

## Fields

| Field                                                                            | Type                                                                             | Required                                                                         | Description                                                                      |
| -------------------------------------------------------------------------------- | -------------------------------------------------------------------------------- | -------------------------------------------------------------------------------- | -------------------------------------------------------------------------------- |
| `information`                                                                    | [models.InformationResponseDto](../models/information-response-dto.md)[]         | :heavy_check_mark:                                                               | N/A                                                                              |
| `responseData`                                                                   | [models.ResponseData](../models/response-data.md)                                | :heavy_check_mark:                                                               | N/A                                                                              |
| `status`                                                                         | [models.AsyncTaskResponseDtoStatus](../models/async-task-response-dto-status.md) | :heavy_check_mark:                                                               | N/A                                                                              |