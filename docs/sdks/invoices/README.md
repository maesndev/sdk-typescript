# Accounting.Invoices

## Overview

### Available Operations

* [updateLineItem](#updatelineitem)

## updateLineItem

### Example Usage

<!-- UsageSnippet language="typescript" operationID="patchLineItem" method="patch" path="/accounting/invoices/{invoiceId}/lineItems/{lineItemId}" -->
```typescript
import { Maesn } from "maesn";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
});

async function run() {
  const result = await maesn.accounting.invoices.updateLineItem({
    invoiceId: "<id>",
    lineItemId: "<id>",
    body: {
      accountCode: "<value>",
      description: "boo in vast configuration navigate as ew who decode",
      discountItemPercentage: 434.56,
      grossAmount: 6604.43,
      itemId: "<id>",
      name: "<value>",
      quantity: 7893.01,
      taxCode: "<value>",
      taxRatePercentage: 4240.25,
      taxType: "<value>",
      type: "MATERIAL",
      unitAmount: 9494.82,
      unitName: "<value>",
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
import { accountingInvoicesUpdateLineItem } from "maesn/funcs/accounting-invoices-update-line-item.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
});

async function run() {
  const res = await accountingInvoicesUpdateLineItem(maesn, {
    invoiceId: "<id>",
    lineItemId: "<id>",
    body: {
      accountCode: "<value>",
      description: "boo in vast configuration navigate as ew who decode",
      discountItemPercentage: 434.56,
      grossAmount: 6604.43,
      itemId: "<id>",
      name: "<value>",
      quantity: 7893.01,
      taxCode: "<value>",
      taxRatePercentage: 4240.25,
      taxType: "<value>",
      type: "MATERIAL",
      unitAmount: 9494.82,
      unitName: "<value>",
    },
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("accountingInvoicesUpdateLineItem failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.PatchLineItemRequest](../../models/operations/patch-line-item-request.md)                                                                                          | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.PatchLineItemResponse](../../models/operations/patch-line-item-response.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |