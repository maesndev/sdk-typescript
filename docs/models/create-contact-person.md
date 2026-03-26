# CreateContactPerson

## Example Usage

```typescript
import { CreateContactPerson } from "@maesn/typescript-sdk/models";

let value: CreateContactPerson = {
  emailAddresses: [
    "<value 1>",
  ],
  firstName: "Charlie",
  lastName: "Schuster",
};
```

## Fields

| Field              | Type               | Required           | Description        |
| ------------------ | ------------------ | ------------------ | ------------------ |
| `emailAddresses`   | *string*[]         | :heavy_check_mark: | N/A                |
| `firstName`        | *string*           | :heavy_check_mark: | N/A                |
| `lastName`         | *string*           | :heavy_check_mark: | N/A                |
| `phoneNumbers`     | *string*[]         | :heavy_minus_sign: | N/A                |
| `salutation`       | *string*           | :heavy_minus_sign: | N/A                |