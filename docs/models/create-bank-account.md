# CreateBankAccount

## Example Usage

```typescript
import { CreateBankAccount } from "maesn/models";

let value: CreateBankAccount = {
  bic: "<value>",
  holder: "<value>",
  isMainAccount: true,
  iban: "LB1029823R2X92I6161X7183KB04",
  name: "<value>",
  sepa: true,
};
```

## Fields

| Field              | Type               | Required           | Description        |
| ------------------ | ------------------ | ------------------ | ------------------ |
| `bic`              | *string*           | :heavy_check_mark: | N/A                |
| `holder`           | *string*           | :heavy_check_mark: | N/A                |
| `isMainAccount`    | *boolean*          | :heavy_check_mark: | N/A                |
| `iban`             | *string*           | :heavy_check_mark: | N/A                |
| `name`             | *string*           | :heavy_check_mark: | N/A                |
| `sepa`             | *boolean*          | :heavy_check_mark: | N/A                |