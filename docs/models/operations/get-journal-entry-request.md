# GetJournalEntryRequest

## Example Usage

```typescript
import { GetJournalEntryRequest } from "maesn/models/operations";

let value: GetJournalEntryRequest = {
  journalEntryId: "<id>",
};
```

## Fields

| Field              | Type               | Required           | Description        |
| ------------------ | ------------------ | ------------------ | ------------------ |
| `journalEntryId`   | *string*           | :heavy_check_mark: | N/A                |
| `environmentName`  | *string*           | :heavy_minus_sign: | N/A                |
| `companyId`        | *string*           | :heavy_minus_sign: | N/A                |
| `journalCode`      | *string*           | :heavy_minus_sign: | N/A                |
| `rawData`          | *boolean*          | :heavy_minus_sign: | N/A                |
| `xApiKey`          | *string*           | :heavy_minus_sign: | API key            |
| `xAccountKey`      | *string*           | :heavy_minus_sign: | Account key        |