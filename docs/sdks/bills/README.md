# Bills

## Overview

### Available Operations

* [update](#update)
* [getLineItems](#getlineitems)

## update

### Example Usage

<!-- UsageSnippet language="typescript" operationID="updateBill" method="put" path="/accounting/bills/{billId}" -->
```typescript
import { Maesn } from "maesn";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
});

async function run() {
  const result = await maesn.bills.update({
    billId: "<id>",
    body: {
      accountId: "<id>",
      addresses: [
        {
          addressLine1: "568 Katheryn Mount",
          addressLine2: "-",
          city: "Schroederfield",
          countryCode: "DZ",
          postalCode: "76990-7129",
          type: "SELLING",
        },
      ],
      billDate: "<value>",
      billNumber: "<value>",
      contactId: "<id>",
      currency: "Seychelles Rupee",
      deliveryDate: "<value>",
      dueDate: "<value>",
      fileId: "<id>",
      journalCode: "<value>",
      lineItems: [],
      name: "<value>",
      oneLineAddress: "<value>",
      paidDate: {},
      paymentTermCode: "<value>",
      paymentStatus: "CREDIT_NOTE_CLEARED",
      paymentDays: 8786.55,
      reference: "<value>",
      shippingDate: {},
      shippingType: "SERVICE_PERIOD",
      status: "PARTIALLY_OVERDUE",
      taxRule: "PHOTOVOLTAIC_EQUIPMENT",
      taxText: "<value>",
      totalDiscountAmount: 1868,
      totalDiscountPercentage: 2539.72,
      totalGrossAmount: 7350.84,
      totalNetAmount: 9819.49,
      totalTaxAmount: 7917.2,
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
import { billsUpdate } from "maesn/funcs/bills-update.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
});

async function run() {
  const res = await billsUpdate(maesn, {
    billId: "<id>",
    body: {
      accountId: "<id>",
      addresses: [
        {
          addressLine1: "568 Katheryn Mount",
          addressLine2: "-",
          city: "Schroederfield",
          countryCode: "DZ",
          postalCode: "76990-7129",
          type: "SELLING",
        },
      ],
      billDate: "<value>",
      billNumber: "<value>",
      contactId: "<id>",
      currency: "Seychelles Rupee",
      deliveryDate: "<value>",
      dueDate: "<value>",
      fileId: "<id>",
      journalCode: "<value>",
      lineItems: [],
      name: "<value>",
      oneLineAddress: "<value>",
      paidDate: {},
      paymentTermCode: "<value>",
      paymentStatus: "CREDIT_NOTE_CLEARED",
      paymentDays: 8786.55,
      reference: "<value>",
      shippingDate: {},
      shippingType: "SERVICE_PERIOD",
      status: "PARTIALLY_OVERDUE",
      taxRule: "PHOTOVOLTAIC_EQUIPMENT",
      taxText: "<value>",
      totalDiscountAmount: 1868,
      totalDiscountPercentage: 2539.72,
      totalGrossAmount: 7350.84,
      totalNetAmount: 9819.49,
      totalTaxAmount: 7917.2,
    },
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("billsUpdate failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.UpdateBillRequest](../../models/operations/update-bill-request.md)                                                                                                 | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.UpdateBillResponse](../../models/operations/update-bill-response.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |

## getLineItems

### Example Usage

<!-- UsageSnippet language="typescript" operationID="getBillLineItems" method="get" path="/accounting/bills/{billId}/lineItems" -->
```typescript
import { Maesn } from "maesn";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
});

async function run() {
  const result = await maesn.bills.getLineItems({
    billId: "<id>",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { MaesnCore } from "maesn/core.js";
import { billsGetLineItems } from "maesn/funcs/bills-get-line-items.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
});

async function run() {
  const res = await billsGetLineItems(maesn, {
    billId: "<id>",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("billsGetLineItems failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.GetBillLineItemsRequest](../../models/operations/get-bill-line-items-request.md)                                                                                   | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.GetBillLineItemsResponse](../../models/operations/get-bill-line-items-response.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |