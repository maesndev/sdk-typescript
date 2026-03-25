# AccountingV2

## Overview

### Available Operations

* [createBookingProposal](#createbookingproposal)
* [createContact](#createcontact)
* [updateContact](#updatecontact)
* [obtainDimensions](#obtaindimensions)

## createBookingProposal

### Example Usage

<!-- UsageSnippet language="typescript" operationID="createBookingProposalV2" method="post" path="/accounting/v2/bookingProposals" -->
```typescript
import { Maesn } from "maesn";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
  security: {
    apiKey: process.env["MAESN_API_KEY"] ?? "",
    accountKey: process.env["MAESN_ACCOUNT_KEY"] ?? "",
  },
});

async function run() {
  const result = await maesn.accountingV2.createBookingProposal({
    body: {},
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { MaesnCore } from "maesn/core.js";
import { accountingV2CreateBookingProposal } from "maesn/funcs/accounting-v2-create-booking-proposal.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
  security: {
    apiKey: process.env["MAESN_API_KEY"] ?? "",
    accountKey: process.env["MAESN_ACCOUNT_KEY"] ?? "",
  },
});

async function run() {
  const res = await accountingV2CreateBookingProposal(maesn, {
    body: {},
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("accountingV2CreateBookingProposal failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.CreateBookingProposalV2Request](../../models/operations/create-booking-proposal-v2-request.md)                                                                     | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.CreateBookingProposalV2Response](../../models/operations/create-booking-proposal-v2-response.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |

## createContact

### Example Usage

<!-- UsageSnippet language="typescript" operationID="createContactV2" method="post" path="/accounting/v2/contacts" -->
```typescript
import { Maesn } from "maesn";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
  security: {
    apiKey: process.env["MAESN_API_KEY"] ?? "",
    accountKey: process.env["MAESN_ACCOUNT_KEY"] ?? "",
  },
});

async function run() {
  const result = await maesn.accountingV2.createContact({
    body: {
      id: "<id>",
      addresses: [],
      companyName: "Adams - Altenwerth",
      contactPersons: [],
      contactType: "CONTACT_PERSON",
      emailAddresses: [
        {
          email: "Karine91@hotmail.com",
          type: "INVOICE",
        },
      ],
      isCustomer: true,
      isSupplier: true,
      number: "<value>",
      phoneNumbers: [
        {
          number: "<value>",
          type: "WHATSAPP",
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
import { accountingV2CreateContact } from "maesn/funcs/accounting-v2-create-contact.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
  security: {
    apiKey: process.env["MAESN_API_KEY"] ?? "",
    accountKey: process.env["MAESN_ACCOUNT_KEY"] ?? "",
  },
});

async function run() {
  const res = await accountingV2CreateContact(maesn, {
    body: {
      id: "<id>",
      addresses: [],
      companyName: "Adams - Altenwerth",
      contactPersons: [],
      contactType: "CONTACT_PERSON",
      emailAddresses: [
        {
          email: "Karine91@hotmail.com",
          type: "INVOICE",
        },
      ],
      isCustomer: true,
      isSupplier: true,
      number: "<value>",
      phoneNumbers: [
        {
          number: "<value>",
          type: "WHATSAPP",
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
    console.log("accountingV2CreateContact failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.CreateContactV2Request](../../models/operations/create-contact-v2-request.md)                                                                                      | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.CreateContactV2Response](../../models/operations/create-contact-v2-response.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |

## updateContact

### Example Usage

<!-- UsageSnippet language="typescript" operationID="putContactV2" method="put" path="/accounting/v2/contacts/{contactId}" -->
```typescript
import { Maesn } from "maesn";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
  security: {
    apiKey: process.env["MAESN_API_KEY"] ?? "",
    accountKey: process.env["MAESN_ACCOUNT_KEY"] ?? "",
  },
});

async function run() {
  const result = await maesn.accountingV2.updateContact({
    contactId: "<id>",
    body: {
      id: "<id>",
      addresses: [],
      companyName: "Rogahn, Cartwright and Waters",
      contactPersons: [],
      contactType: "CONTACT_PERSON",
      emailAddresses: [
        {
          email: "Kaleigh58@yahoo.com",
          type: "OTHER",
        },
      ],
      isCustomer: false,
      isSupplier: true,
      number: "<value>",
      phoneNumbers: [],
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
import { accountingV2UpdateContact } from "maesn/funcs/accounting-v2-update-contact.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
  security: {
    apiKey: process.env["MAESN_API_KEY"] ?? "",
    accountKey: process.env["MAESN_ACCOUNT_KEY"] ?? "",
  },
});

async function run() {
  const res = await accountingV2UpdateContact(maesn, {
    contactId: "<id>",
    body: {
      id: "<id>",
      addresses: [],
      companyName: "Rogahn, Cartwright and Waters",
      contactPersons: [],
      contactType: "CONTACT_PERSON",
      emailAddresses: [
        {
          email: "Kaleigh58@yahoo.com",
          type: "OTHER",
        },
      ],
      isCustomer: false,
      isSupplier: true,
      number: "<value>",
      phoneNumbers: [],
      projectId: "<id>",
      website: "<value>",
    },
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("accountingV2UpdateContact failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.PutContactV2Request](../../models/operations/put-contact-v2-request.md)                                                                                            | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.PutContactV2Response](../../models/operations/put-contact-v2-response.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |

## obtainDimensions

### Example Usage

<!-- UsageSnippet language="typescript" operationID="getDimensionsV2" method="get" path="/accounting/v2/dimensions" -->
```typescript
import { Maesn } from "maesn";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
  security: {
    apiKey: process.env["MAESN_API_KEY"] ?? "",
    accountKey: process.env["MAESN_ACCOUNT_KEY"] ?? "",
  },
});

async function run() {
  const result = await maesn.accountingV2.obtainDimensions();

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { MaesnCore } from "maesn/core.js";
import { accountingV2ObtainDimensions } from "maesn/funcs/accounting-v2-obtain-dimensions.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
  security: {
    apiKey: process.env["MAESN_API_KEY"] ?? "",
    accountKey: process.env["MAESN_ACCOUNT_KEY"] ?? "",
  },
});

async function run() {
  const res = await accountingV2ObtainDimensions(maesn);
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("accountingV2ObtainDimensions failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.GetDimensionsV2Request](../../models/operations/get-dimensions-v2-request.md)                                                                                      | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.GetDimensionsV2Response](../../models/operations/get-dimensions-v2-response.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |