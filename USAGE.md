<!-- Start SDK Example Usage [usage] -->
```typescript
import { Maesn } from "@maesn/typescript-sdk";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
  security: {
    option1: {
      apiKey: process.env["MAESN_API_KEY"] ?? "",
      accountKey: process.env["MAESN_ACCOUNT_KEY"] ?? "",
    },
  },
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