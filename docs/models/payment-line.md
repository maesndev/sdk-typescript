# PaymentLine

## Example Usage

```typescript
import { PaymentLine } from "@maesn/typescript-sdk/models";

let value: PaymentLine = {
  accountId: "<id>",
  amount: 278.6,
  contactName: "<value>",
  description: "intently likely before vet enthusiastically tough aircraft",
  invoiceId: "<id>",
  supplierId: "<id>",
  paymentDate: "<value>",
};
```

## Fields

| Field              | Type               | Required           | Description        |
| ------------------ | ------------------ | ------------------ | ------------------ |
| `accountId`        | *string*           | :heavy_check_mark: | N/A                |
| `amount`           | *number*           | :heavy_check_mark: | N/A                |
| `contactName`      | *string*           | :heavy_check_mark: | N/A                |
| `contactId`        | *string*           | :heavy_minus_sign: | N/A                |
| `customerId`       | *string*           | :heavy_minus_sign: | N/A                |
| `description`      | *string*           | :heavy_check_mark: | N/A                |
| `invoiceId`        | *string*           | :heavy_check_mark: | N/A                |
| `supplierId`       | *string*           | :heavy_check_mark: | N/A                |
| `paymentDate`      | *string*           | :heavy_check_mark: | N/A                |