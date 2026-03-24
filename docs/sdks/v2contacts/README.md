# Accounting.V2.Contacts

## Overview

### Available Operations

* [update](#update)

## update

### Example Usage

<!-- UsageSnippet language="typescript" operationID="patchContactV2" method="patch" path="/accounting/v2/contacts/{contactId}" -->
```typescript
import { Maesn } from "maesn";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
});

async function run() {
  const result = await maesn.accounting.v2.contacts.update({
    contactId: "<id>",
    body: {
      id: "<id>",
      addresses: [],
      companyName: "Kassulke - Schaden",
      contactPersons: [
        {
          id: "<id>",
          emailAddresses: [
            {
              email: "Jolie44@yahoo.com",
              type: "PAYMENT",
            },
          ],
          firstName: "Fritz",
          lastName: "Buckridge",
          phoneNumbers: [],
          salutation: "<value>",
        },
      ],
      contactType: "COMPANY",
      emailAddresses: [],
      isCustomer: true,
      isSupplier: false,
      number: "<value>",
      phoneNumbers: [
        {
          number: "<value>",
          type: "LANDLINE",
        },
      ],
      projectId: "<id>",
      website: "<value>",
    },
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { MaesnCore } from "maesn/core.js";
import { accountingV2ContactsUpdate } from "maesn/funcs/accounting-v2-contacts-update.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
});

async function run() {
  const res = await accountingV2ContactsUpdate(maesn, {
    contactId: "<id>",
    body: {
      id: "<id>",
      addresses: [],
      companyName: "Kassulke - Schaden",
      contactPersons: [
        {
          id: "<id>",
          emailAddresses: [
            {
              email: "Jolie44@yahoo.com",
              type: "PAYMENT",
            },
          ],
          firstName: "Fritz",
          lastName: "Buckridge",
          phoneNumbers: [],
          salutation: "<value>",
        },
      ],
      contactType: "COMPANY",
      emailAddresses: [],
      isCustomer: true,
      isSupplier: false,
      number: "<value>",
      phoneNumbers: [
        {
          number: "<value>",
          type: "LANDLINE",
        },
      ],
      projectId: "<id>",
      website: "<value>",
    },
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("accountingV2ContactsUpdate failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.PatchContactV2Request](../../models/operations/patch-contact-v2-request.md)                                                                                        | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.PatchContactV2Response](../../models/operations/patch-contact-v2-response.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |