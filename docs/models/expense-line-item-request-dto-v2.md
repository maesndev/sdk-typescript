# ExpenseLineItemRequestDtoV2

## Example Usage

```typescript
import { ExpenseLineItemRequestDtoV2 } from "@maesn/typescript-sdk/models";

let value: ExpenseLineItemRequestDtoV2 = {};
```

## Fields

| Field                                                                                | Type                                                                                 | Required                                                                             | Description                                                                          |
| ------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------ |
| `id`                                                                                 | *string*                                                                             | :heavy_minus_sign:                                                                   | N/A                                                                                  |
| `account`                                                                            | [models.AccountRequestCommonDtoV2](../models/account-request-common-dto-v2.md)       | :heavy_minus_sign:                                                                   | N/A                                                                                  |
| `currency`                                                                           | *string*                                                                             | :heavy_minus_sign:                                                                   | N/A                                                                                  |
| `description`                                                                        | *string*                                                                             | :heavy_minus_sign:                                                                   | N/A                                                                                  |
| `dimensions`                                                                         | [models.DimensionRequestCommonDtoV2](../models/dimension-request-common-dto-v2.md)[] | :heavy_minus_sign:                                                                   | N/A                                                                                  |
| `documentNumber`                                                                     | *string*                                                                             | :heavy_minus_sign:                                                                   | N/A                                                                                  |
| `exchangeRate`                                                                       | *number*                                                                             | :heavy_minus_sign:                                                                   | N/A                                                                                  |
| `itemId`                                                                             | *string*                                                                             | :heavy_minus_sign:                                                                   | N/A                                                                                  |
| `taxRate`                                                                            | [models.TaxRateRequestDtoV2](../models/tax-rate-request-dto-v2.md)                   | :heavy_minus_sign:                                                                   | N/A                                                                                  |
| `totalGrossAmount`                                                                   | *number*                                                                             | :heavy_minus_sign:                                                                   | N/A                                                                                  |
| `totalNetAmount`                                                                     | *number*                                                                             | :heavy_minus_sign:                                                                   | N/A                                                                                  |