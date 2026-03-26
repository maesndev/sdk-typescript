# Accounting.Bills

## Overview

### Available Operations

* [addLineItem](#addlineitem)

## addLineItem

### Example Usage

<!-- UsageSnippet language="typescript" operationID="createBillLineItem" method="post" path="/accounting/bills/{billId}/lineItems" -->
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
  const result = await maesn.accounting.bills.addLineItem({
    billId: "<id>",
    body: {
      id: "<id>",
      accountId: "<id>",
      accountNumber: "<value>",
      deferredEndDate: "<value>",
      deferredStartDate: "<value>",
      description: "scented truthfully on mid creak hmph huzzah warlike section",
      dimensions: [],
      itemId: "<id>",
      itemName: "<value>",
      quantity: 5032.18,
      taxCode: "<value>",
      taxRatePercentage: 3223.82,
      totalDiscountAmount: 9726.16,
      totalDiscountPercentage: 263.97,
      totalGrossAmount: 8391.76,
      totalNetAmount: 8035.68,
      totalTaxAmount: 3841.55,
      unitAmount: 5672.84,
      unitDiscountAmount: 749.8,
      unitDiscountPercentage: 1350.66,
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
import { accountingBillsAddLineItem } from "maesn/funcs/accounting-bills-add-line-item.js";

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
  const res = await accountingBillsAddLineItem(maesn, {
    billId: "<id>",
    body: {
      id: "<id>",
      accountId: "<id>",
      accountNumber: "<value>",
      deferredEndDate: "<value>",
      deferredStartDate: "<value>",
      description: "scented truthfully on mid creak hmph huzzah warlike section",
      dimensions: [],
      itemId: "<id>",
      itemName: "<value>",
      quantity: 5032.18,
      taxCode: "<value>",
      taxRatePercentage: 3223.82,
      totalDiscountAmount: 9726.16,
      totalDiscountPercentage: 263.97,
      totalGrossAmount: 8391.76,
      totalNetAmount: 8035.68,
      totalTaxAmount: 3841.55,
      unitAmount: 5672.84,
      unitDiscountAmount: 749.8,
      unitDiscountPercentage: 1350.66,
      unitName: "<value>",
    },
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("accountingBillsAddLineItem failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.CreateBillLineItemRequest](../../models/operations/create-bill-line-item-request.md)                                                                               | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.CreateBillLineItemResponse](../../models/operations/create-bill-line-item-response.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |