<!-- Start SDK Example Usage [usage] -->
```typescript
import { Maesn } from "@maesn/typescript-sdk";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
  apiKey: "<value>",
  accountKey: "<value>",
});

async function run() {
  const result = await maesn.accounting.getAccount({
    accountId: "<id>",
  });

  console.log(result);
}

run();

```
<!-- End SDK Example Usage [usage] -->