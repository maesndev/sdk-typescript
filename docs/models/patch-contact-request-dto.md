# PatchContactRequestDto

## Example Usage

```typescript
import { PatchContactRequestDto } from "@maesn/typescript-sdk/models";

let value: PatchContactRequestDto = {};
```

## Fields

| Field                                                                                           | Type                                                                                            | Required                                                                                        | Description                                                                                     |
| ----------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------- |
| `contactType`                                                                                   | [models.PatchContactRequestDtoContactType](../models/patch-contact-request-dto-contact-type.md) | :heavy_minus_sign:                                                                              | N/A                                                                                             |
| `companyName`                                                                                   | *string*                                                                                        | :heavy_minus_sign:                                                                              | N/A                                                                                             |
| `contactPersons`                                                                                | [models.PatchContactPerson](../models/patch-contact-person.md)[]                                | :heavy_minus_sign:                                                                              | N/A                                                                                             |
| `addresses`                                                                                     | [models.PatchContactAddress](../models/patch-contact-address.md)[]                              | :heavy_minus_sign:                                                                              | N/A                                                                                             |
| `emailAddresses`                                                                                | [models.CreateEmailAddress](../models/create-email-address.md)[]                                | :heavy_minus_sign:                                                                              | N/A                                                                                             |
| `phoneNumbers`                                                                                  | [models.CreatePhoneNumber](../models/create-phone-number.md)[]                                  | :heavy_minus_sign:                                                                              | N/A                                                                                             |
| `bankAccount`                                                                                   | [models.BankAccount](../models/bank-account.md)                                                 | :heavy_minus_sign:                                                                              | N/A                                                                                             |
| `projectId`                                                                                     | *string*                                                                                        | :heavy_minus_sign:                                                                              | N/A                                                                                             |