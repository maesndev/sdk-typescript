# Webhooks

## Overview

### Available Operations

* [createWebhookEndUser](#createwebhookenduser)
* [deleteWebhookEndUser](#deletewebhookenduser)
* [createWebhook](#createwebhook)
* [getWebhooks](#getwebhooks)
* [deleteWebhook](#deletewebhook)

## createWebhookEndUser

### Example Usage

<!-- UsageSnippet language="typescript" operationID="createWebhookEndUser" method="post" path="/webhooks/user" -->
```typescript
import { Maesn } from "@maesn/typescript-sdk";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
  apiKey: "<value>",
  accountKey: "<value>",
});

async function run() {
  const result = await maesn.webhooks.createWebhookEndUser({
    body: {
      callbackUrl: "https://oddball-subsidy.com/",
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
import { webhooksCreateWebhookEndUser } from "@maesn/typescript-sdk/funcs/webhooks-create-webhook-end-user.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
  apiKey: "<value>",
  accountKey: "<value>",
});

async function run() {
  const res = await webhooksCreateWebhookEndUser(maesn, {
    body: {
      callbackUrl: "https://oddball-subsidy.com/",
    },
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("webhooksCreateWebhookEndUser failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.CreateWebhookEndUserRequest](../../models/operations/create-webhook-end-user-request.md)                                                                           | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.CreateWebhookEndUserResponse](../../models/operations/create-webhook-end-user-response.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |

## deleteWebhookEndUser

### Example Usage

<!-- UsageSnippet language="typescript" operationID="deleteWebhookEndUser" method="delete" path="/webhooks/user/{webhookId}" -->
```typescript
import { Maesn } from "@maesn/typescript-sdk";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
  apiKey: "<value>",
  accountKey: "<value>",
});

async function run() {
  const result = await maesn.webhooks.deleteWebhookEndUser({
    webhookId: "<id>",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { MaesnCore } from "@maesn/typescript-sdk/core.js";
import { webhooksDeleteWebhookEndUser } from "@maesn/typescript-sdk/funcs/webhooks-delete-webhook-end-user.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
  apiKey: "<value>",
  accountKey: "<value>",
});

async function run() {
  const res = await webhooksDeleteWebhookEndUser(maesn, {
    webhookId: "<id>",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("webhooksDeleteWebhookEndUser failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.DeleteWebhookEndUserRequest](../../models/operations/delete-webhook-end-user-request.md)                                                                           | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.DeleteWebhookEndUserResponse](../../models/operations/delete-webhook-end-user-response.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |

## createWebhook

### Example Usage

<!-- UsageSnippet language="typescript" operationID="createWebhook" method="post" path="/webhooks" -->
```typescript
import { Maesn } from "@maesn/typescript-sdk";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
  apiKey: "<value>",
  accountKey: "<value>",
});

async function run() {
  const result = await maesn.webhooks.createWebhook({
    body: {
      callbackUrl: "https://experienced-sailor.biz/",
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
import { webhooksCreateWebhook } from "@maesn/typescript-sdk/funcs/webhooks-create-webhook.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
  apiKey: "<value>",
  accountKey: "<value>",
});

async function run() {
  const res = await webhooksCreateWebhook(maesn, {
    body: {
      callbackUrl: "https://experienced-sailor.biz/",
    },
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("webhooksCreateWebhook failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.CreateWebhookRequest](../../models/operations/create-webhook-request.md)                                                                                           | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.CreateWebhookResponse](../../models/operations/create-webhook-response.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |

## getWebhooks

### Example Usage

<!-- UsageSnippet language="typescript" operationID="getWebhooks" method="get" path="/webhooks" -->
```typescript
import { Maesn } from "@maesn/typescript-sdk";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
  apiKey: "<value>",
  accountKey: "<value>",
});

async function run() {
  const result = await maesn.webhooks.getWebhooks();

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { MaesnCore } from "@maesn/typescript-sdk/core.js";
import { webhooksGetWebhooks } from "@maesn/typescript-sdk/funcs/webhooks-get-webhooks.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
  apiKey: "<value>",
  accountKey: "<value>",
});

async function run() {
  const res = await webhooksGetWebhooks(maesn);
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("webhooksGetWebhooks failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.GetWebhooksRequest](../../models/operations/get-webhooks-request.md)                                                                                               | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.GetWebhooksResponse](../../models/operations/get-webhooks-response.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |

## deleteWebhook

### Example Usage

<!-- UsageSnippet language="typescript" operationID="deleteWebhook" method="delete" path="/webhooks/{webhookId}" -->
```typescript
import { Maesn } from "@maesn/typescript-sdk";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
  apiKey: "<value>",
  accountKey: "<value>",
});

async function run() {
  const result = await maesn.webhooks.deleteWebhook({
    webhookId: "<id>",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { MaesnCore } from "@maesn/typescript-sdk/core.js";
import { webhooksDeleteWebhook } from "@maesn/typescript-sdk/funcs/webhooks-delete-webhook.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
  apiKey: "<value>",
  accountKey: "<value>",
});

async function run() {
  const res = await webhooksDeleteWebhook(maesn, {
    webhookId: "<id>",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("webhooksDeleteWebhook failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.DeleteWebhookRequest](../../models/operations/delete-webhook-request.md)                                                                                           | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.DeleteWebhookResponse](../../models/operations/delete-webhook-response.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |