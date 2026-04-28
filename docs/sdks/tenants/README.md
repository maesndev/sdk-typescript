# Tenants

## Overview

### Available Operations

* [systemRegistration](#systemregistration)
* [addCallbackUrl](#addcallbackurl)
* [getEndUserList](#getenduserlist)
* [countEndUsersBySystem](#countendusersbysystem)
* [deleteEndUser](#deleteenduser)
* [getCallbackUrl](#getcallbackurl)
* [getRegisteredSystems](#getregisteredsystems)
* [getTargetSystemValues](#gettargetsystemvalues)
* [getTargetSystemRequirements](#gettargetsystemrequirements)
* [getRegisteredSystemsMasked](#getregisteredsystemsmasked)
* [deleteRegisteredSystem](#deleteregisteredsystem)
* [getSubmissionPageStyle](#getsubmissionpagestyle)
* [updateSubmissionPageStyle](#updatesubmissionpagestyle)
* [getSubmissionPageStyleByKey](#getsubmissionpagestylebykey)
* [generateTenantSigningSecret](#generatetenantsigningsecret)

## systemRegistration

### Example Usage

<!-- UsageSnippet language="typescript" operationID="systemRegistration" method="post" path="/tenants/register-system" -->
```typescript
import { Maesn } from "@maesn/typescript-sdk";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
  apiKey: "<value>",
  accountKey: "<value>",
});

async function run() {
  const result = await maesn.tenants.systemRegistration({
    body: {
      targetSystem: "<value>",
      clientId: "<id>",
      clientSecret: "<value>",
      customValues: [
        {
          key: "<key>",
          value: "<value>",
        },
      ],
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
import { tenantsSystemRegistration } from "@maesn/typescript-sdk/funcs/tenants-system-registration.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
  apiKey: "<value>",
  accountKey: "<value>",
});

async function run() {
  const res = await tenantsSystemRegistration(maesn, {
    body: {
      targetSystem: "<value>",
      clientId: "<id>",
      clientSecret: "<value>",
      customValues: [
        {
          key: "<key>",
          value: "<value>",
        },
      ],
    },
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("tenantsSystemRegistration failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.SystemRegistrationRequest](../../models/operations/system-registration-request.md)                                                                                 | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[string](../../models/.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |

## addCallbackUrl

### Example Usage

<!-- UsageSnippet language="typescript" operationID="addCallbackUrl" method="post" path="/tenants/add-callback-urls" -->
```typescript
import { Maesn } from "@maesn/typescript-sdk";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
  apiKey: "<value>",
  accountKey: "<value>",
});

async function run() {
  const result = await maesn.tenants.addCallbackUrl({
    body: {
      callbackUrl: "https://steep-tuber.net/",
      cancelCallbackUrl: "https://tight-sideboard.com/",
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
import { tenantsAddCallbackUrl } from "@maesn/typescript-sdk/funcs/tenants-add-callback-url.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
  apiKey: "<value>",
  accountKey: "<value>",
});

async function run() {
  const res = await tenantsAddCallbackUrl(maesn, {
    body: {
      callbackUrl: "https://steep-tuber.net/",
      cancelCallbackUrl: "https://tight-sideboard.com/",
    },
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("tenantsAddCallbackUrl failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.AddCallbackUrlRequest](../../models/operations/add-callback-url-request.md)                                                                                        | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[string](../../models/.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |

## getEndUserList

### Example Usage

<!-- UsageSnippet language="typescript" operationID="getEndUserList" method="get" path="/tenants/get-end-user-list" -->
```typescript
import { Maesn } from "@maesn/typescript-sdk";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
  apiKey: "<value>",
  accountKey: "<value>",
});

async function run() {
  const result = await maesn.tenants.getEndUserList();

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { MaesnCore } from "@maesn/typescript-sdk/core.js";
import { tenantsGetEndUserList } from "@maesn/typescript-sdk/funcs/tenants-get-end-user-list.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
  apiKey: "<value>",
  accountKey: "<value>",
});

async function run() {
  const res = await tenantsGetEndUserList(maesn);
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("tenantsGetEndUserList failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.GetEndUserListRequest](../../models/operations/get-end-user-list-request.md)                                                                                       | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[models.BaseResponseDto](../../models/base-response-dto.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |

## countEndUsersBySystem

### Example Usage

<!-- UsageSnippet language="typescript" operationID="countEndUsersBySystem" method="get" path="/tenants/count-end-users-by-system" -->
```typescript
import { Maesn } from "@maesn/typescript-sdk";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
  apiKey: "<value>",
  accountKey: "<value>",
});

async function run() {
  const result = await maesn.tenants.countEndUsersBySystem();

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { MaesnCore } from "@maesn/typescript-sdk/core.js";
import { tenantsCountEndUsersBySystem } from "@maesn/typescript-sdk/funcs/tenants-count-end-users-by-system.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
  apiKey: "<value>",
  accountKey: "<value>",
});

async function run() {
  const res = await tenantsCountEndUsersBySystem(maesn);
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("tenantsCountEndUsersBySystem failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.CountEndUsersBySystemRequest](../../models/operations/count-end-users-by-system-request.md)                                                                        | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[models.BaseResponseDto](../../models/base-response-dto.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |

## deleteEndUser

### Example Usage

<!-- UsageSnippet language="typescript" operationID="deleteEndUser" method="delete" path="/tenants/delete-end-user" -->
```typescript
import { Maesn } from "@maesn/typescript-sdk";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
  apiKey: "<value>",
  accountKey: "<value>",
});

async function run() {
  const result = await maesn.tenants.deleteEndUser();

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { MaesnCore } from "@maesn/typescript-sdk/core.js";
import { tenantsDeleteEndUser } from "@maesn/typescript-sdk/funcs/tenants-delete-end-user.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
  apiKey: "<value>",
  accountKey: "<value>",
});

async function run() {
  const res = await tenantsDeleteEndUser(maesn);
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("tenantsDeleteEndUser failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.DeleteEndUserRequest](../../models/operations/delete-end-user-request.md)                                                                                          | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.DeleteEndUserResponse](../../models/operations/delete-end-user-response.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |

## getCallbackUrl

### Example Usage

<!-- UsageSnippet language="typescript" operationID="getCallbackUrl" method="get" path="/tenants/get-callback-url" -->
```typescript
import { Maesn } from "@maesn/typescript-sdk";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
  apiKey: "<value>",
  accountKey: "<value>",
});

async function run() {
  const result = await maesn.tenants.getCallbackUrl();

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { MaesnCore } from "@maesn/typescript-sdk/core.js";
import { tenantsGetCallbackUrl } from "@maesn/typescript-sdk/funcs/tenants-get-callback-url.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
  apiKey: "<value>",
  accountKey: "<value>",
});

async function run() {
  const res = await tenantsGetCallbackUrl(maesn);
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("tenantsGetCallbackUrl failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.GetCallbackUrlRequest](../../models/operations/get-callback-url-request.md)                                                                                        | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[models.BaseResponseDto](../../models/base-response-dto.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |

## getRegisteredSystems

### Example Usage

<!-- UsageSnippet language="typescript" operationID="getRegisteredSystems" method="get" path="/tenants/get-registered-systems" -->
```typescript
import { Maesn } from "@maesn/typescript-sdk";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
  apiKey: "<value>",
  accountKey: "<value>",
});

async function run() {
  const result = await maesn.tenants.getRegisteredSystems();

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { MaesnCore } from "@maesn/typescript-sdk/core.js";
import { tenantsGetRegisteredSystems } from "@maesn/typescript-sdk/funcs/tenants-get-registered-systems.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
  apiKey: "<value>",
  accountKey: "<value>",
});

async function run() {
  const res = await tenantsGetRegisteredSystems(maesn);
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("tenantsGetRegisteredSystems failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.GetRegisteredSystemsRequest](../../models/operations/get-registered-systems-request.md)                                                                            | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[models.BaseResponseDto](../../models/base-response-dto.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |

## getTargetSystemValues

### Example Usage

<!-- UsageSnippet language="typescript" operationID="getTargetSystemValues" method="get" path="/tenants/get-target-system-values" -->
```typescript
import { Maesn } from "@maesn/typescript-sdk";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
  apiKey: "<value>",
  accountKey: "<value>",
});

async function run() {
  const result = await maesn.tenants.getTargetSystemValues();

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { MaesnCore } from "@maesn/typescript-sdk/core.js";
import { tenantsGetTargetSystemValues } from "@maesn/typescript-sdk/funcs/tenants-get-target-system-values.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
  apiKey: "<value>",
  accountKey: "<value>",
});

async function run() {
  const res = await tenantsGetTargetSystemValues(maesn);
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("tenantsGetTargetSystemValues failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.GetTargetSystemValuesRequest](../../models/operations/get-target-system-values-request.md)                                                                         | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[models.BaseResponseDto](../../models/base-response-dto.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |

## getTargetSystemRequirements

### Example Usage

<!-- UsageSnippet language="typescript" operationID="getTargetSystemRequirements" method="get" path="/tenants/get-target-system-requirements" -->
```typescript
import { Maesn } from "@maesn/typescript-sdk";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
  apiKey: "<value>",
  accountKey: "<value>",
});

async function run() {
  const result = await maesn.tenants.getTargetSystemRequirements();

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { MaesnCore } from "@maesn/typescript-sdk/core.js";
import { tenantsGetTargetSystemRequirements } from "@maesn/typescript-sdk/funcs/tenants-get-target-system-requirements.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
  apiKey: "<value>",
  accountKey: "<value>",
});

async function run() {
  const res = await tenantsGetTargetSystemRequirements(maesn);
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("tenantsGetTargetSystemRequirements failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.GetTargetSystemRequirementsRequest](../../models/operations/get-target-system-requirements-request.md)                                                             | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[models.BaseResponseDto](../../models/base-response-dto.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |

## getRegisteredSystemsMasked

### Example Usage

<!-- UsageSnippet language="typescript" operationID="getRegisteredSystemsMasked" method="get" path="/tenants/get-registered-systems-masked" -->
```typescript
import { Maesn } from "@maesn/typescript-sdk";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
  apiKey: "<value>",
  accountKey: "<value>",
});

async function run() {
  const result = await maesn.tenants.getRegisteredSystemsMasked();

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { MaesnCore } from "@maesn/typescript-sdk/core.js";
import { tenantsGetRegisteredSystemsMasked } from "@maesn/typescript-sdk/funcs/tenants-get-registered-systems-masked.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
  apiKey: "<value>",
  accountKey: "<value>",
});

async function run() {
  const res = await tenantsGetRegisteredSystemsMasked(maesn);
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("tenantsGetRegisteredSystemsMasked failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.GetRegisteredSystemsMaskedRequest](../../models/operations/get-registered-systems-masked-request.md)                                                               | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[models.BaseResponseDto](../../models/base-response-dto.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |

## deleteRegisteredSystem

### Example Usage

<!-- UsageSnippet language="typescript" operationID="deleteRegisteredSystem" method="delete" path="/tenants/delete-registered-system/{targetSystem}" -->
```typescript
import { Maesn } from "@maesn/typescript-sdk";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
  apiKey: "<value>",
  accountKey: "<value>",
});

async function run() {
  const result = await maesn.tenants.deleteRegisteredSystem({
    targetSystem: "<value>",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { MaesnCore } from "@maesn/typescript-sdk/core.js";
import { tenantsDeleteRegisteredSystem } from "@maesn/typescript-sdk/funcs/tenants-delete-registered-system.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
  apiKey: "<value>",
  accountKey: "<value>",
});

async function run() {
  const res = await tenantsDeleteRegisteredSystem(maesn, {
    targetSystem: "<value>",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("tenantsDeleteRegisteredSystem failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.DeleteRegisteredSystemRequest](../../models/operations/delete-registered-system-request.md)                                                                        | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[string](../../models/.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |

## getSubmissionPageStyle

### Example Usage

<!-- UsageSnippet language="typescript" operationID="getSubmissionPageStyle" method="get" path="/tenants/get-submission-page-style" -->
```typescript
import { Maesn } from "@maesn/typescript-sdk";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
  apiKey: "<value>",
  accountKey: "<value>",
});

async function run() {
  const result = await maesn.tenants.getSubmissionPageStyle({
    code: "<value>",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { MaesnCore } from "@maesn/typescript-sdk/core.js";
import { tenantsGetSubmissionPageStyle } from "@maesn/typescript-sdk/funcs/tenants-get-submission-page-style.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
  apiKey: "<value>",
  accountKey: "<value>",
});

async function run() {
  const res = await tenantsGetSubmissionPageStyle(maesn, {
    code: "<value>",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("tenantsGetSubmissionPageStyle failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.GetSubmissionPageStyleRequest](../../models/operations/get-submission-page-style-request.md)                                                                       | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.GetSubmissionPageStyleResponse](../../models/operations/get-submission-page-style-response.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |

## updateSubmissionPageStyle

### Example Usage

<!-- UsageSnippet language="typescript" operationID="updateSubmissionPageStyle" method="post" path="/tenants/submission-page-style" -->
```typescript
import { Maesn } from "@maesn/typescript-sdk";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
  apiKey: "<value>",
  accountKey: "<value>",
});

async function run() {
  const result = await maesn.tenants.updateSubmissionPageStyle({
    body: {
      logoSvg: "<value>",
      logoPng: "<value>",
      backgroundColor: "<value>",
      titleColor: "<value>",
      textColor: "<value>",
      inputBackgroundColor: "<value>",
      submitButtonColor: "<value>",
      cancelButtonColor: "<value>",
      errorTextColor: "<value>",
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
import { tenantsUpdateSubmissionPageStyle } from "@maesn/typescript-sdk/funcs/tenants-update-submission-page-style.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
  apiKey: "<value>",
  accountKey: "<value>",
});

async function run() {
  const res = await tenantsUpdateSubmissionPageStyle(maesn, {
    body: {
      logoSvg: "<value>",
      logoPng: "<value>",
      backgroundColor: "<value>",
      titleColor: "<value>",
      textColor: "<value>",
      inputBackgroundColor: "<value>",
      submitButtonColor: "<value>",
      cancelButtonColor: "<value>",
      errorTextColor: "<value>",
    },
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("tenantsUpdateSubmissionPageStyle failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.UpdateSubmissionPageStyleRequest](../../models/operations/update-submission-page-style-request.md)                                                                 | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.UpdateSubmissionPageStyleResponse](../../models/operations/update-submission-page-style-response.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |

## getSubmissionPageStyleByKey

### Example Usage

<!-- UsageSnippet language="typescript" operationID="getSubmissionPageStyleByKey" method="get" path="/tenants/submission-page-style-by-key" -->
```typescript
import { Maesn } from "@maesn/typescript-sdk";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
  apiKey: "<value>",
  accountKey: "<value>",
});

async function run() {
  const result = await maesn.tenants.getSubmissionPageStyleByKey();

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { MaesnCore } from "@maesn/typescript-sdk/core.js";
import { tenantsGetSubmissionPageStyleByKey } from "@maesn/typescript-sdk/funcs/tenants-get-submission-page-style-by-key.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
  apiKey: "<value>",
  accountKey: "<value>",
});

async function run() {
  const res = await tenantsGetSubmissionPageStyleByKey(maesn);
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("tenantsGetSubmissionPageStyleByKey failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.GetSubmissionPageStyleByKeyRequest](../../models/operations/get-submission-page-style-by-key-request.md)                                                           | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.GetSubmissionPageStyleByKeyResponse](../../models/operations/get-submission-page-style-by-key-response.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |

## generateTenantSigningSecret

### Example Usage

<!-- UsageSnippet language="typescript" operationID="generateTenantSigningSecret" method="post" path="/tenants/signing-secret" -->
```typescript
import { Maesn } from "@maesn/typescript-sdk";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
  apiKey: "<value>",
  accountKey: "<value>",
});

async function run() {
  const result = await maesn.tenants.generateTenantSigningSecret();

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { MaesnCore } from "@maesn/typescript-sdk/core.js";
import { tenantsGenerateTenantSigningSecret } from "@maesn/typescript-sdk/funcs/tenants-generate-tenant-signing-secret.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
  apiKey: "<value>",
  accountKey: "<value>",
});

async function run() {
  const res = await tenantsGenerateTenantSigningSecret(maesn);
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("tenantsGenerateTenantSigningSecret failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.GenerateTenantSigningSecretRequest](../../models/operations/generate-tenant-signing-secret-request.md)                                                             | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.GenerateTenantSigningSecretResponse](../../models/operations/generate-tenant-signing-secret-response.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |