# JournalEntries

## Overview

### Available Operations

* [createBulk](#createbulk)

## createBulk

### Example Usage

<!-- UsageSnippet language="typescript" operationID="createJournalEntries" method="post" path="/accounting/journalEntries/bulk" -->
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
  const result = await maesn.journalEntries.createBulk({
    body: {
      accountNumberLength: 1703.63,
      chartOfAccount: "SKR14",
      entries: [
        {
          accountId: "<id>",
          accountingPeriodId: "<id>",
          currency: "UYU",
          debitCreditIndicator: "CREDIT",
          deliveryDate: "<value>",
          description: "duh whose wherever dusk",
          documentId: "<id>",
          dueDate: "<value>",
          exchangeRate: "<value>",
          isProvisional: false,
          journalCode: "<value>",
          journalLineItems: [
            {
              accountCode: "<value>",
              accountId: "<id>",
              accountNumber: 8284.89,
              currency: "MOP",
              customerId: "<id>",
              debitCreditIndicator: "DEBIT",
              description: "thoughtfully blah membership nor dress gosh summarise vein",
              dimensions: [
                "<value 1>",
              ],
              discountAmount: 8088.09,
              documentNumber: "<value>",
              exchangeRate: "<value>",
              supplierId: "<id>",
              taxRate: {
                id: "<id>",
                code: "<value>",
                name: "<value>",
                taxRatePercentage: "<value>",
              },
              thirdPartyCode: "<value>",
              totalGrossAmount: 6768.04,
              totalNetAmount: 8076.41,
              totalTaxAmount: 7880.01,
            },
          ],
          journalType: "<value>",
          number: "<value>",
          taxAssignmentDate: "<value>",
          transactionDate: "<value>",
        },
      ],
      fiscalYearStartDate: "<value>",
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
import { journalEntriesCreateBulk } from "maesn/funcs/journal-entries-create-bulk.js";

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
  const res = await journalEntriesCreateBulk(maesn, {
    body: {
      accountNumberLength: 1703.63,
      chartOfAccount: "SKR14",
      entries: [
        {
          accountId: "<id>",
          accountingPeriodId: "<id>",
          currency: "UYU",
          debitCreditIndicator: "CREDIT",
          deliveryDate: "<value>",
          description: "duh whose wherever dusk",
          documentId: "<id>",
          dueDate: "<value>",
          exchangeRate: "<value>",
          isProvisional: false,
          journalCode: "<value>",
          journalLineItems: [
            {
              accountCode: "<value>",
              accountId: "<id>",
              accountNumber: 8284.89,
              currency: "MOP",
              customerId: "<id>",
              debitCreditIndicator: "DEBIT",
              description: "thoughtfully blah membership nor dress gosh summarise vein",
              dimensions: [
                "<value 1>",
              ],
              discountAmount: 8088.09,
              documentNumber: "<value>",
              exchangeRate: "<value>",
              supplierId: "<id>",
              taxRate: {
                id: "<id>",
                code: "<value>",
                name: "<value>",
                taxRatePercentage: "<value>",
              },
              thirdPartyCode: "<value>",
              totalGrossAmount: 6768.04,
              totalNetAmount: 8076.41,
              totalTaxAmount: 7880.01,
            },
          ],
          journalType: "<value>",
          number: "<value>",
          taxAssignmentDate: "<value>",
          transactionDate: "<value>",
        },
      ],
      fiscalYearStartDate: "<value>",
    },
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("journalEntriesCreateBulk failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.CreateJournalEntriesRequest](../../models/operations/create-journal-entries-request.md)                                                                            | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.CreateJournalEntriesResponse](../../models/operations/create-journal-entries-response.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |