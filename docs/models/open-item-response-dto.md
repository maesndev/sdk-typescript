# OpenItemResponseDto

## Example Usage

```typescript
import { OpenItemResponseDto } from "maesn/models";

let value: OpenItemResponseDto = {
  id: "<id>",
  accountId: "<id>",
  accountName: "<value>",
  accountNumber: "<value>",
  createdDate: "<value>",
  currency: "Uzbekistan Sum",
  documentNumber: "<value>",
  entries: [],
  openBalance: {
    amount: 7475.92,
    debitCreditIndicator: "DEBIT",
  },
  postingDate: "<value>",
  totalCreditAmount: 8912.43,
  totalDebitAmount: 7025.66,
  type: "BILL",
  updatedDate: "<value>",
};
```

## Fields

| Field                                                                          | Type                                                                           | Required                                                                       | Description                                                                    |
| ------------------------------------------------------------------------------ | ------------------------------------------------------------------------------ | ------------------------------------------------------------------------------ | ------------------------------------------------------------------------------ |
| `id`                                                                           | *string*                                                                       | :heavy_check_mark:                                                             | N/A                                                                            |
| `accountId`                                                                    | *string*                                                                       | :heavy_check_mark:                                                             | N/A                                                                            |
| `accountName`                                                                  | *string*                                                                       | :heavy_check_mark:                                                             | N/A                                                                            |
| `accountNumber`                                                                | *string*                                                                       | :heavy_check_mark:                                                             | N/A                                                                            |
| `createdDate`                                                                  | *string*                                                                       | :heavy_check_mark:                                                             | N/A                                                                            |
| `currency`                                                                     | *string*                                                                       | :heavy_check_mark:                                                             | N/A                                                                            |
| `documentNumber`                                                               | *string*                                                                       | :heavy_check_mark:                                                             | N/A                                                                            |
| `entries`                                                                      | [models.OpenItemEntryResponseDto](../models/open-item-entry-response-dto.md)[] | :heavy_check_mark:                                                             | N/A                                                                            |
| `openBalance`                                                                  | [models.Balance](../models/balance.md)                                         | :heavy_check_mark:                                                             | N/A                                                                            |
| `postingDate`                                                                  | *string*                                                                       | :heavy_check_mark:                                                             | N/A                                                                            |
| `totalCreditAmount`                                                            | *number*                                                                       | :heavy_check_mark:                                                             | N/A                                                                            |
| `totalDebitAmount`                                                             | *number*                                                                       | :heavy_check_mark:                                                             | N/A                                                                            |
| `type`                                                                         | [models.OpenItemResponseDtoType](../models/open-item-response-dto-type.md)     | :heavy_check_mark:                                                             | N/A                                                                            |
| `updatedDate`                                                                  | *string*                                                                       | :heavy_check_mark:                                                             | N/A                                                                            |