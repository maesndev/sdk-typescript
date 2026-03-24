# CreateContactPersonDtoV2

## Example Usage

```typescript
import { CreateContactPersonDtoV2 } from "maesn/models";

let value: CreateContactPersonDtoV2 = {
  id: "<id>",
  emailAddresses: [],
  firstName: "Dimitri",
  lastName: "Franecki",
  phoneNumbers: [
    {
      number: "<value>",
      type: "LANDLINE",
    },
  ],
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