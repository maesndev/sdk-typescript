# GetLineItemRequest

## Example Usage

```typescript
import { GetLineItemRequest } from "maesn/models/operations";

let value: GetLineItemRequest = {
  invoiceId: "<id>",
  lineItemId: "<id>",
};
```

## Fields

| Field              | Type               | Required           | Description        |
| ------------------ | ------------------ | ------------------ | ------------------ |
| `invoiceId`        | *string*           | :heavy_check_mark: | N/A                |
| `lineItemId`       | *string*           | :heavy_check_mark: | N/A                |
| `environmentName`  | *string*           | :heavy_minus_sign: | N/A                |
| `companyId`        | *string*           | :heavy_minus_sign: | N/A                |
| `rawData`          | *boolean*          | :heavy_minus_sign: | N/A                |