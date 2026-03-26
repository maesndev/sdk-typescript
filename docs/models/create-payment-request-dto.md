# CreatePaymentRequestDto

## Example Usage

```typescript
import { CreatePaymentRequestDto } from "@maesn/typescript-sdk/models";

let value: CreatePaymentRequestDto = {};
```

## Fields

| Field                                                                                               | Type                                                                                                | Required                                                                                            | Description                                                                                         |
| --------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------- |
| `currency`                                                                                          | *string*                                                                                            | :heavy_minus_sign:                                                                                  | N/A                                                                                                 |
| `documentType`                                                                                      | [models.CreatePaymentRequestDtoDocumentType](../models/create-payment-request-dto-document-type.md) | :heavy_minus_sign:                                                                                  | N/A                                                                                                 |
| `exchangeRate`                                                                                      | *number*                                                                                            | :heavy_minus_sign:                                                                                  | N/A                                                                                                 |
| `journalCode`                                                                                       | *string*                                                                                            | :heavy_minus_sign:                                                                                  | N/A                                                                                                 |
| `paymentType`                                                                                       | *string*                                                                                            | :heavy_minus_sign:                                                                                  | N/A                                                                                                 |
| `paymentLines`                                                                                      | [models.CreatePaymentLine](../models/create-payment-line.md)[]                                      | :heavy_minus_sign:                                                                                  | N/A                                                                                                 |