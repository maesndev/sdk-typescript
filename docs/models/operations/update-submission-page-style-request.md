# UpdateSubmissionPageStyleRequest

## Example Usage

```typescript
import { UpdateSubmissionPageStyleRequest } from "@maesn/typescript-sdk/models/operations";

let value: UpdateSubmissionPageStyleRequest = {
  body: {
    logoSvg: "<value>",
    logoPng: "<value>",
    backgroundColor: "<value>",
    titleColor: "<value>",
    textColor: "<value>",
    inputBackgroundColor: "<value>",
    submitButtonColor: "<value>",
    cancelButtonColor: "<value>",
    errorTextColor: "<value>",
  },
};
```

## Fields

| Field                                                                      | Type                                                                       | Required                                                                   | Description                                                                |
| -------------------------------------------------------------------------- | -------------------------------------------------------------------------- | -------------------------------------------------------------------------- | -------------------------------------------------------------------------- |
| `apiKey`                                                                   | *string*                                                                   | :heavy_minus_sign:                                                         | API key                                                                    |
| `accountKey`                                                               | *string*                                                                   | :heavy_minus_sign:                                                         | Account key                                                                |
| `body`                                                                     | [models.SubmissionPageStyleDto](../../models/submission-page-style-dto.md) | :heavy_check_mark:                                                         | N/A                                                                        |