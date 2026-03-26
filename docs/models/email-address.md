# EmailAddress

## Example Usage

```typescript
import { EmailAddress } from "@maesn/typescript-sdk/models";

let value: EmailAddress = {
  email: "Mike_McClure17@gmail.com",
  type: "INVOICE",
};
```

## Fields

| Field                                                      | Type                                                       | Required                                                   | Description                                                |
| ---------------------------------------------------------- | ---------------------------------------------------------- | ---------------------------------------------------------- | ---------------------------------------------------------- |
| `email`                                                    | *string*                                                   | :heavy_check_mark:                                         | N/A                                                        |
| `type`                                                     | [models.EmailAddressType](../models/email-address-type.md) | :heavy_check_mark:                                         | N/A                                                        |