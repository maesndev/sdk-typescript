# GetPurchaseOrderLineItemRequest

## Example Usage

```typescript
import { GetPurchaseOrderLineItemRequest } from "maesn/models/operations";

let value: GetPurchaseOrderLineItemRequest = {
  purchaseOrderId: "<id>",
  lineItemId: "<id>",
};
```

## Fields

| Field              | Type               | Required           | Description        |
| ------------------ | ------------------ | ------------------ | ------------------ |
| `purchaseOrderId`  | *string*           | :heavy_check_mark: | N/A                |
| `lineItemId`       | *string*           | :heavy_check_mark: | N/A                |
| `environmentName`  | *string*           | :heavy_minus_sign: | N/A                |
| `companyId`        | *string*           | :heavy_minus_sign: | N/A                |
| `rawData`          | *boolean*          | :heavy_minus_sign: | N/A                |
| `xApiKey`          | *string*           | :heavy_minus_sign: | API key            |
| `xAccountKey`      | *string*           | :heavy_minus_sign: | Account key        |