# CreateAccountRequestDto

## Example Usage

```typescript
import { CreateAccountRequestDto } from "maesn/models";

let value: CreateAccountRequestDto = {
  balance: 245.79,
  class: "EXPENSE",
  code: "<value>",
  currency: "BWP",
  description: "boldly among bonfire",
  name: "<value>",
  number: "<value>",
  parentAccountId: "<id>",
  status: "ARCHIVED",
  type: "OTHER",
};
```

## Fields

| Field                                                                                      | Type                                                                                       | Required                                                                                   | Description                                                                                |
| ------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------ |
| `balance`                                                                                  | *number*                                                                                   | :heavy_check_mark:                                                                         | N/A                                                                                        |
| `class`                                                                                    | [models.CreateAccountRequestDtoClass](../models/create-account-request-dto-class.md)       | :heavy_check_mark:                                                                         | N/A                                                                                        |
| `code`                                                                                     | *string*                                                                                   | :heavy_check_mark:                                                                         | N/A                                                                                        |
| `currency`                                                                                 | [models.CreateAccountRequestDtoCurrency](../models/create-account-request-dto-currency.md) | :heavy_check_mark:                                                                         | N/A                                                                                        |
| `description`                                                                              | *string*                                                                                   | :heavy_check_mark:                                                                         | N/A                                                                                        |
| `name`                                                                                     | *string*                                                                                   | :heavy_check_mark:                                                                         | N/A                                                                                        |
| `number`                                                                                   | *string*                                                                                   | :heavy_check_mark:                                                                         | N/A                                                                                        |
| `parentAccountId`                                                                          | *string*                                                                                   | :heavy_check_mark:                                                                         | N/A                                                                                        |
| `status`                                                                                   | [models.CreateAccountRequestDtoStatus](../models/create-account-request-dto-status.md)     | :heavy_check_mark:                                                                         | N/A                                                                                        |
| `type`                                                                                     | [models.CreateAccountRequestDtoType](../models/create-account-request-dto-type.md)         | :heavy_check_mark:                                                                         | N/A                                                                                        |