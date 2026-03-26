# OpenBalance

## Example Usage

```typescript
import { OpenBalance } from "@maesn/typescript-sdk/models";

let value: OpenBalance = {
  amount: 3253.63,
  debitCreditIndicator: "CREDIT",
};
```

## Fields

| Field                                                                                                        | Type                                                                                                         | Required                                                                                                     | Description                                                                                                  |
| ------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------ |
| `amount`                                                                                                     | *number*                                                                                                     | :heavy_check_mark:                                                                                           | N/A                                                                                                          |
| `debitCreditIndicator`                                                                                       | [models.OpenItemResponseDtoDebitCreditIndicator](../models/open-item-response-dto-debit-credit-indicator.md) | :heavy_check_mark:                                                                                           | N/A                                                                                                          |