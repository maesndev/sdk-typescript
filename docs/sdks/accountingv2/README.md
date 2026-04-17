# AccountingV2

## Overview

### Available Operations

* [createBookingProposalV2](#createbookingproposalv2)
* [getContactsV2](#getcontactsv2)
* [createContactV2](#createcontactv2)
* [getContactV2](#getcontactv2)
* [putContactV2](#putcontactv2)
* [patchContactV2](#patchcontactv2)
* [getDimensionsV2](#getdimensionsv2)
* [getDimensionsByDimension](#getdimensionsbydimension)

## createBookingProposalV2

### Example Usage

<!-- UsageSnippet language="typescript" operationID="createBookingProposalV2" method="post" path="/accounting/v2/bookingProposals" -->
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
  const result = await maesn.accountingV2.createBookingProposalV2({
    body: {},
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { MaesnCore } from "@maesn/typescript-sdk/core.js";
import { accountingV2CreateBookingProposalV2 } from "@maesn/typescript-sdk/funcs/accounting-v2-create-booking-proposal-v2.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
  security: {
    option1: {
      apiKey: process.env["MAESN_API_KEY"] ?? "",
      accountKey: process.env["MAESN_ACCOUNT_KEY"] ?? "",
    },
  },
});

async function run() {
  const res = await accountingV2CreateBookingProposalV2(maesn, {
    body: {},
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("accountingV2CreateBookingProposalV2 failed:", res.error);
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

## getContactsV2

### Example Usage

<!-- UsageSnippet language="typescript" operationID="getContactsV2" method="get" path="/accounting/v2/contacts" -->
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
  const result = await maesn.accountingV2.getContactsV2();

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { MaesnCore } from "@maesn/typescript-sdk/core.js";
import { accountingV2GetContactsV2 } from "@maesn/typescript-sdk/funcs/accounting-v2-get-contacts-v2.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
  security: {
    option1: {
      apiKey: process.env["MAESN_API_KEY"] ?? "",
      accountKey: process.env["MAESN_ACCOUNT_KEY"] ?? "",
    },
  },
});

async function run() {
  const res = await accountingV2GetContactsV2(maesn);
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("accountingV2GetContactsV2 failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.GetContactsV2Request](../../models/operations/get-contacts-v2-request.md)                                                                                          | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.GetContactsV2Response](../../models/operations/get-contacts-v2-response.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |

## createContactV2

### Example Usage

<!-- UsageSnippet language="typescript" operationID="createContactV2" method="post" path="/accounting/v2/contacts" -->
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
  const result = await maesn.accountingV2.createContactV2({
    body: {
      contactType: "CONTACT_PERSON",
    },
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { MaesnCore } from "@maesn/typescript-sdk/core.js";
import { accountingV2CreateContactV2 } from "@maesn/typescript-sdk/funcs/accounting-v2-create-contact-v2.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
  security: {
    option1: {
      apiKey: process.env["MAESN_API_KEY"] ?? "",
      accountKey: process.env["MAESN_ACCOUNT_KEY"] ?? "",
    },
  },
});

async function run() {
  const res = await accountingV2CreateContactV2(maesn, {
    body: {
      contactType: "CONTACT_PERSON",
    },
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("accountingV2CreateContactV2 failed:", res.error);
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

## getContactV2

### Example Usage

<!-- UsageSnippet language="typescript" operationID="getContactV2" method="get" path="/accounting/v2/contacts/{contactId}" -->
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
  const result = await maesn.accountingV2.getContactV2({
    contactId: "<id>",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { MaesnCore } from "@maesn/typescript-sdk/core.js";
import { accountingV2GetContactV2 } from "@maesn/typescript-sdk/funcs/accounting-v2-get-contact-v2.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
  security: {
    option1: {
      apiKey: process.env["MAESN_API_KEY"] ?? "",
      accountKey: process.env["MAESN_ACCOUNT_KEY"] ?? "",
    },
  },
});

async function run() {
  const res = await accountingV2GetContactV2(maesn, {
    contactId: "<id>",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("accountingV2GetContactV2 failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.GetContactV2Request](../../models/operations/get-contact-v2-request.md)                                                                                            | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.GetContactV2Response](../../models/operations/get-contact-v2-response.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |

## putContactV2

### Example Usage

<!-- UsageSnippet language="typescript" operationID="putContactV2" method="put" path="/accounting/v2/contacts/{contactId}" -->
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
  const result = await maesn.accountingV2.putContactV2({
    contactId: "<id>",
    body: {
      contactType: "CONTACT_PERSON",
    },
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { MaesnCore } from "@maesn/typescript-sdk/core.js";
import { accountingV2PutContactV2 } from "@maesn/typescript-sdk/funcs/accounting-v2-put-contact-v2.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
  security: {
    option1: {
      apiKey: process.env["MAESN_API_KEY"] ?? "",
      accountKey: process.env["MAESN_ACCOUNT_KEY"] ?? "",
    },
  },
});

async function run() {
  const res = await accountingV2PutContactV2(maesn, {
    contactId: "<id>",
    body: {
      contactType: "CONTACT_PERSON",
    },
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("accountingV2PutContactV2 failed:", res.error);
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

## patchContactV2

### Example Usage

<!-- UsageSnippet language="typescript" operationID="patchContactV2" method="patch" path="/accounting/v2/contacts/{contactId}" -->
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
  const result = await maesn.accountingV2.patchContactV2({
    contactId: "<id>",
    body: {
      contactType: "COMPANY",
    },
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { MaesnCore } from "@maesn/typescript-sdk/core.js";
import { accountingV2PatchContactV2 } from "@maesn/typescript-sdk/funcs/accounting-v2-patch-contact-v2.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
  security: {
    option1: {
      apiKey: process.env["MAESN_API_KEY"] ?? "",
      accountKey: process.env["MAESN_ACCOUNT_KEY"] ?? "",
    },
  },
});

async function run() {
  const res = await accountingV2PatchContactV2(maesn, {
    contactId: "<id>",
    body: {
      contactType: "COMPANY",
    },
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("accountingV2PatchContactV2 failed:", res.error);
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

## getDimensionsV2

### Example Usage

<!-- UsageSnippet language="typescript" operationID="getDimensionsV2" method="get" path="/accounting/v2/dimensions" -->
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
  const result = await maesn.accountingV2.getDimensionsV2();

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { MaesnCore } from "@maesn/typescript-sdk/core.js";
import { accountingV2GetDimensionsV2 } from "@maesn/typescript-sdk/funcs/accounting-v2-get-dimensions-v2.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
  security: {
    option1: {
      apiKey: process.env["MAESN_API_KEY"] ?? "",
      accountKey: process.env["MAESN_ACCOUNT_KEY"] ?? "",
    },
  },
});

async function run() {
  const res = await accountingV2GetDimensionsV2(maesn);
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("accountingV2GetDimensionsV2 failed:", res.error);
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

## getDimensionsByDimension

### Example Usage

<!-- UsageSnippet language="typescript" operationID="getDimensionsByDimension" method="get" path="/accounting/v2/dimensions/{dimension}" -->
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
  const result = await maesn.accountingV2.getDimensionsByDimension({
    dimension: "<value>",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { MaesnCore } from "@maesn/typescript-sdk/core.js";
import { accountingV2GetDimensionsByDimension } from "@maesn/typescript-sdk/funcs/accounting-v2-get-dimensions-by-dimension.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
  security: {
    option1: {
      apiKey: process.env["MAESN_API_KEY"] ?? "",
      accountKey: process.env["MAESN_ACCOUNT_KEY"] ?? "",
    },
  },
});

async function run() {
  const res = await accountingV2GetDimensionsByDimension(maesn, {
    dimension: "<value>",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("accountingV2GetDimensionsByDimension failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.GetDimensionsByDimensionRequest](../../models/operations/get-dimensions-by-dimension-request.md)                                                                   | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.GetDimensionsByDimensionResponse](../../models/operations/get-dimensions-by-dimension-response.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |