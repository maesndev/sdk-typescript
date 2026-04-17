# User

## Overview

### Available Operations

* [getUserInfo](#getuserinfo)

## getUserInfo

### Example Usage

<!-- UsageSnippet language="typescript" operationID="getUserInfo" method="get" path="/user/user-info" -->
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
  const result = await maesn.user.getUserInfo();

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { MaesnCore } from "@maesn/typescript-sdk/core.js";
import { userGetUserInfo } from "@maesn/typescript-sdk/funcs/user-get-user-info.js";

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
  const res = await userGetUserInfo(maesn);
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("userGetUserInfo failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.GetUserInfoResponse](../../models/operations/get-user-info-response.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |