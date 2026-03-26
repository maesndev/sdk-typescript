# OpenItemResponseDto

## Example Usage

```typescript
import { OpenItemResponseDto } from "@maesn/typescript-sdk/models";

let value: OpenItemResponseDto = {
  id: "<id>",
  accountId: "<id>",
  accountName: "<value>",
  accountNumber: "<value>",
  createdDate: "<value>",
  currency: "Bhutanese Ngultrum",
  documentNumber: null,
  entries: [
    {
      amount: 5551.37,
      currency: "Gourde",
      debitCreditIndicator: "CREDIT",
      description: null,
      dueDate: "<value>",
      postingDate: "<value>",
    },
  ],
  openBalance: {
    amount: 9260.14,
    debitCreditIndicator: "CREDIT",
  },
  postingDate: "<value>",
  totalCreditAmount: 4740.94,
  totalDebitAmount: 682.06,
  type: "INVOICE",
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
| `openBalance`                                                                  | [models.OpenBalance](../models/open-balance.md)                                | :heavy_check_mark:                                                             | N/A                                                                            |
| `postingDate`                                                                  | *string*                                                                       | :heavy_check_mark:                                                             | N/A                                                                            |
| `totalCreditAmount`                                                            | *number*                                                                       | :heavy_check_mark:                                                             | N/A                                                                            |
| `totalDebitAmount`                                                             | *number*                                                                       | :heavy_check_mark:                                                             | N/A                                                                            |
| `type`                                                                         | [models.OpenItemResponseDtoType](../models/open-item-response-dto-type.md)     | :heavy_check_mark:                                                             | N/A                                                                            |
| `updatedDate`                                                                  | *string*                                                                       | :heavy_check_mark:                                                             | N/A                                                                            |