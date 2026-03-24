# ContactPersonDtoV2

## Example Usage

```typescript
import { ContactPersonDtoV2 } from "maesn/models";

let value: ContactPersonDtoV2 = {
  id: "<id>",
  emailAddresses: [
    {
      email: "Amira56@gmail.com",
      type: "PRIVATE",
    },
  ],
  firstName: "Lesley",
  lastName: "Champlin",
  phoneNumbers: [],
  salutation: "<value>",
};
```

## Fields

| Field                                               | Type                                                | Required                                            | Description                                         |
| --------------------------------------------------- | --------------------------------------------------- | --------------------------------------------------- | --------------------------------------------------- |
| `id`                                                | *string*                                            | :heavy_check_mark:                                  | N/A                                                 |
| `emailAddresses`                                    | [models.EmailAddress](../models/email-address.md)[] | :heavy_check_mark:                                  | N/A                                                 |
| `firstName`                                         | *string*                                            | :heavy_check_mark:                                  | N/A                                                 |
| `lastName`                                          | *string*                                            | :heavy_check_mark:                                  | N/A                                                 |
| `phoneNumbers`                                      | [models.PhoneNumber](../models/phone-number.md)[]   | :heavy_check_mark:                                  | N/A                                                 |
| `salutation`                                        | *string*                                            | :heavy_check_mark:                                  | N/A                                                 |