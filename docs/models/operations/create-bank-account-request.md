# CreateBankAccountRequest

## Example Usage

```typescript
import { CreateBankAccountRequest } from "maesn/models/operations";

let value: CreateBankAccountRequest = {
  body: {
    balance: 7802.65,
    bankName: "<value>",
    bic: "<value>",
    currency: "PLN",
    description:
      "lest within oxygenate noted object exaggerate excluding physical pile",
    fileType: "CSV",
    iban: "GT50J02H7Y9P35TK78X0K8732M07",
    name: "<value>",
    number: "<value>",
    system: "<value>",
    status: "ACTIVE",
    type: "YEAR_END_REFLECTION",
  },
};
```

## Fields

| Field                                                                                 | Type                                                                                  | Required                                                                              | Description                                                                           |
| ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- |
| `environmentName`                                                                     | *string*                                                                              | :heavy_minus_sign:                                                                    | N/A                                                                                   |
| `companyId`                                                                           | *string*                                                                              | :heavy_minus_sign:                                                                    | N/A                                                                                   |
| `xApiKey`                                                                             | *string*                                                                              | :heavy_minus_sign:                                                                    | API key                                                                               |
| `xAccountKey`                                                                         | *string*                                                                              | :heavy_minus_sign:                                                                    | Account key                                                                           |
| `body`                                                                                | [models.CreateBankAccountRequestDto](../../models/create-bank-account-request-dto.md) | :heavy_check_mark:                                                                    | N/A                                                                                   |