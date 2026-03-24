# JournalEntryAttachments

## Overview

### Available Operations

* [getById](#getbyid)

## getById

### Example Usage

<!-- UsageSnippet language="typescript" operationID="getJournalEntryAttachmentById" method="get" path="/accounting/journalEntries/{journalEntryId}/Attachments/{attachmentId}" -->
```typescript
import { Maesn } from "maesn";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
});

async function run() {
  const result = await maesn.journalEntryAttachments.getById({
    journalEntryId: "<id>",
    attachmentId: "<id>",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { MaesnCore } from "maesn/core.js";
import { journalEntryAttachmentsGetById } from "maesn/funcs/journal-entry-attachments-get-by-id.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
});

async function run() {
  const res = await journalEntryAttachmentsGetById(maesn, {
    journalEntryId: "<id>",
    attachmentId: "<id>",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("journalEntryAttachmentsGetById failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.GetJournalEntryAttachmentByIdRequest](../../models/operations/get-journal-entry-attachment-by-id-request.md)                                                       | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.GetJournalEntryAttachmentByIdResponse](../../models/operations/get-journal-entry-attachment-by-id-response.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |