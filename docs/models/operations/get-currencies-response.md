# GetCurrenciesResponse

List of currencies for the authenticated end user's connected target system

## Example Usage

```typescript
import { GetCurrenciesResponse } from "@maesn/typescript-sdk/models/operations";

let value: GetCurrenciesResponse = {
  data: [
    {
      id: null,
      code: "<value>",
      decimalPlaces: 8897.73,
      name: "<value>",
      roundingPrecision: 6355.38,
      updatedDate: null,
    },
  ],
  errors: {},
  rawData: {},
};
```

## Fields

| Field                                                                                 | Type                                                                                  | Required                                                                              | Description                                                                           |
| ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- |
| `meta`                                                                                | [operations.GetCurrenciesMeta](../../models/operations/get-currencies-meta.md)        | :heavy_minus_sign:                                                                    | N/A                                                                                   |
| `data`                                                                                | [models.CurrencyResponseDto](../../models/currency-response-dto.md)[]                 | :heavy_check_mark:                                                                    | N/A                                                                                   |
| `errors`                                                                              | [operations.GetCurrenciesErrors](../../models/operations/get-currencies-errors.md)    | :heavy_check_mark:                                                                    | N/A                                                                                   |
| `rawData`                                                                             | [operations.GetCurrenciesRawData](../../models/operations/get-currencies-raw-data.md) | :heavy_check_mark:                                                                    | N/A                                                                                   |