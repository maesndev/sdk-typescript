# AsyncTaskResponseDto

## Example Usage

```typescript
import { AsyncTaskResponseDto } from "maesn/models";

let value: AsyncTaskResponseDto = {
  information: [
    {
      filename: "example.file",
      message: "<value>",
      timestamp: "<value>",
      type: "<value>",
    },
  ],
  responseData: {},
  status: "DELETED",
};
```

## Fields

| Field                                                                            | Type                                                                             | Required                                                                         | Description                                                                      |
| -------------------------------------------------------------------------------- | -------------------------------------------------------------------------------- | -------------------------------------------------------------------------------- | -------------------------------------------------------------------------------- |
| `information`                                                                    | [models.InformationResponseDto](../models/information-response-dto.md)[]         | :heavy_check_mark:                                                               | N/A                                                                              |
| `responseData`                                                                   | [models.ResponseData](../models/response-data.md)                                | :heavy_check_mark:                                                               | N/A                                                                              |
| `status`                                                                         | [models.AsyncTaskResponseDtoStatus](../models/async-task-response-dto-status.md) | :heavy_check_mark:                                                               | N/A                                                                              |