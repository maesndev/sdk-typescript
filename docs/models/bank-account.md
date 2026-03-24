# BankAccount

## Example Usage

```typescript
import { BankAccount } from "maesn/models";

let value: BankAccount = {
  iban: "LU06009HH90028414217",
  bic: "<value>",
  holder: "<value>",
  sepa: false,
};
```

## Fields

| Field              | Type               | Required           | Description        |
| ------------------ | ------------------ | ------------------ | ------------------ |
| `iban`             | *string*           | :heavy_check_mark: | N/A                |
| `bic`              | *string*           | :heavy_check_mark: | N/A                |
| `holder`           | *string*           | :heavy_check_mark: | N/A                |
| `sepa`             | *boolean*          | :heavy_check_mark: | N/A                |