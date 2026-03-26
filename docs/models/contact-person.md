# ContactPerson

## Example Usage

```typescript
import { ContactPerson } from "@maesn/typescript-sdk/models";

let value: ContactPerson = {
  emailAddresses: [],
  firstName: "Vance",
  lastName: null,
  phoneNumbers: [],
  salutation: "<value>",
};
```

## Fields

| Field                                               | Type                                                | Required                                            | Description                                         |
| --------------------------------------------------- | --------------------------------------------------- | --------------------------------------------------- | --------------------------------------------------- |
| `emailAddresses`                                    | [models.EmailAddress](../models/email-address.md)[] | :heavy_check_mark:                                  | N/A                                                 |
| `firstName`                                         | *string*                                            | :heavy_check_mark:                                  | N/A                                                 |
| `lastName`                                          | *string*                                            | :heavy_check_mark:                                  | N/A                                                 |
| `phoneNumbers`                                      | [models.PhoneNumber](../models/phone-number.md)[]   | :heavy_check_mark:                                  | N/A                                                 |
| `salutation`                                        | *string*                                            | :heavy_check_mark:                                  | N/A                                                 |