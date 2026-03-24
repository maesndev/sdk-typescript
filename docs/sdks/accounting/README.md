# Accounting

## Overview

### Available Operations

* [retrieveAccount](#retrieveaccount)
* [retrieveAccounts](#retrieveaccounts)
* [addAccount](#addaccount)
* [retrieveBankAccounts](#retrievebankaccounts)
* [addBankAccount](#addbankaccount)
* [fetchBankAccount](#fetchbankaccount)
* [retrieveDimensions](#retrievedimensions)
* [recordTransaction](#recordtransaction)
* [fetchCustomers](#fetchcustomers)
* [createCustomer](#createcustomer)
* [fetchCustomer](#fetchcustomer)
* [updateCustomer](#updatecustomer)
* [amendCustomer](#amendcustomer)
* [retrieveSuppliers](#retrievesuppliers)
* [addSupplier](#addsupplier)
* [fetchSupplier](#fetchsupplier)
* [modifySupplier](#modifysupplier)
* [amendSupplier](#amendsupplier)
* [getContacts](#getcontacts)
* [addContact](#addcontact)
* [fetchContact](#fetchcontact)
* [replaceContact](#replacecontact)
* [createContactsBulk](#createcontactsbulk)
* [batchAddContacts](#batchaddcontacts)
* [retrieveInvoices](#retrieveinvoices)
* [addInvoice](#addinvoice)
* [fetchInvoice](#fetchinvoice)
* [amendInvoice](#amendinvoice)
* [fetchInvoiceDocument](#fetchinvoicedocument)
* [uploadFile](#uploadfile)
* [fetchDocumentTypes](#fetchdocumenttypes)
* [getAsyncTask](#getasynctask)
* [retrieveItems](#retrieveitems)
* [fetchItem](#fetchitem)
* [retrieveInvoiceLineItems](#retrieveinvoicelineitems)
* [addInvoiceLineItem](#addinvoicelineitem)
* [retrieveInvoiceLineItem](#retrieveinvoicelineitem)
* [fetchJournals](#fetchjournals)
* [listJournalEntries](#listjournalentries)
* [addJournalEntry](#addjournalentry)
* [fetchJournalEntry](#fetchjournalentry)
* [createJournalEntryAttachments](#createjournalentryattachments)
* [fetchOffers](#fetchoffers)
* [addOffer](#addoffer)
* [fetchOffer](#fetchoffer)
* [fetchOfferLineItems](#fetchofferlineitems)
* [retrieveOfferLineItem](#retrieveofferlineitem)
* [addExpense](#addexpense)
* [fetchExpenses](#fetchexpenses)
* [fetchExpense](#fetchexpense)
* [getProjects](#getprojects)
* [addProject](#addproject)
* [fetchProject](#fetchproject)
* [listSalesOrders](#listsalesorders)
* [addSalesOrder](#addsalesorder)
* [fetchSalesOrder](#fetchsalesorder)
* [listSalesOrderLineItems](#listsalesorderlineitems)
* [getPaymentTerms](#getpaymentterms)
* [addPaymentTerm](#addpaymentterm)
* [fetchPaymentTerm](#fetchpaymentterm)
* [retrieveTaxRates](#retrievetaxrates)
* [fetchTaxRate](#fetchtaxrate)
* [retrievePayments](#retrievepayments)
* [addPayment](#addpayment)
* [fetchPayment](#fetchpayment)
* [removePayment](#removepayment)
* [addEventSubscription](#addeventsubscription)
* [removeEventSubscription](#removeeventsubscription)
* [getProfile](#getprofile)
* [createPassThrough](#createpassthrough)
* [fetchBills](#fetchbills)
* [addBill](#addbill)
* [fetchBill](#fetchbill)
* [removeBill](#removebill)
* [fetchBillDocument](#fetchbilldocument)
* [createBookingProposal](#createbookingproposal)
* [listBookingProposals](#listbookingproposals)
* [retrieveBookingProposal](#retrievebookingproposal)
* [fetchBookingProposalDocument](#fetchbookingproposaldocument)
* [addBooking](#addbooking)
* [retrieveVendorCredits](#retrievevendorcredits)
* [createVendorCredit](#createvendorcredit)
* [modifyVendorCredit](#modifyvendorcredit)
* [modifyBillLineItem](#modifybilllineitem)
* [fetchPurchaseOrder](#fetchpurchaseorder)
* [retrievePurchaseOrderLineItems](#retrievepurchaseorderlineitems)
* [retrievePurchaseOrderLineItem](#retrievepurchaseorderlineitem)
* [getGoodsReceipts](#getgoodsreceipts)
* [retrieveGoodsReceipt](#retrievegoodsreceipt)
* [retrieveGoodsReceiptLineItems](#retrievegoodsreceiptlineitems)
* [fetchUnits](#fetchunits)
* [retrieveOpenItems](#retrieveopenitems)
* [fetchTrialBalance](#fetchtrialbalance)
* [listCreditNotes](#listcreditnotes)
* [fetchCreditNote](#fetchcreditnote)
* [getFiscalYears](#getfiscalyears)

## retrieveAccount

### Example Usage

<!-- UsageSnippet language="typescript" operationID="getAccount" method="get" path="/accounting/accounts/{accountId}" -->
```typescript
import { Maesn } from "maesn";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
});

async function run() {
  const result = await maesn.accounting.retrieveAccount({
    accountId: "<id>",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { MaesnCore } from "maesn/core.js";
import { accountingRetrieveAccount } from "maesn/funcs/accounting-retrieve-account.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
});

async function run() {
  const res = await accountingRetrieveAccount(maesn, {
    accountId: "<id>",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("accountingRetrieveAccount failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.GetAccountRequest](../../models/operations/get-account-request.md)                                                                                                 | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.GetAccountResponse](../../models/operations/get-account-response.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |

## retrieveAccounts

### Example Usage

<!-- UsageSnippet language="typescript" operationID="getAccounts" method="get" path="/accounting/accounts" -->
```typescript
import { Maesn } from "maesn";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
});

async function run() {
  const result = await maesn.accounting.retrieveAccounts();

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { MaesnCore } from "maesn/core.js";
import { accountingRetrieveAccounts } from "maesn/funcs/accounting-retrieve-accounts.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
});

async function run() {
  const res = await accountingRetrieveAccounts(maesn);
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("accountingRetrieveAccounts failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.GetAccountsRequest](../../models/operations/get-accounts-request.md)                                                                                               | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.GetAccountsResponse](../../models/operations/get-accounts-response.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |

## addAccount

### Example Usage

<!-- UsageSnippet language="typescript" operationID="createAccount" method="post" path="/accounting/accounts" -->
```typescript
import { Maesn } from "maesn";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
});

async function run() {
  const result = await maesn.accounting.addAccount({
    body: {
      balance: 8561.8,
      class: "ASSET",
      code: "<value>",
      currency: "PGK",
      description: "only zowie crossly preclude",
      name: "<value>",
      number: "<value>",
      parentAccountId: "<id>",
      status: "ACTIVE",
      type: "STATISTICAL_CONSUMPTION",
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
import { accountingAddAccount } from "maesn/funcs/accounting-add-account.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
});

async function run() {
  const res = await accountingAddAccount(maesn, {
    body: {
      balance: 8561.8,
      class: "ASSET",
      code: "<value>",
      currency: "PGK",
      description: "only zowie crossly preclude",
      name: "<value>",
      number: "<value>",
      parentAccountId: "<id>",
      status: "ACTIVE",
      type: "STATISTICAL_CONSUMPTION",
    },
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("accountingAddAccount failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.CreateAccountRequest](../../models/operations/create-account-request.md)                                                                                           | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.CreateAccountResponse](../../models/operations/create-account-response.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |

## retrieveBankAccounts

### Example Usage

<!-- UsageSnippet language="typescript" operationID="getBankAccounts" method="get" path="/accounting/bankAccounts" -->
```typescript
import { Maesn } from "maesn";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
});

async function run() {
  const result = await maesn.accounting.retrieveBankAccounts();

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { MaesnCore } from "maesn/core.js";
import { accountingRetrieveBankAccounts } from "maesn/funcs/accounting-retrieve-bank-accounts.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
});

async function run() {
  const res = await accountingRetrieveBankAccounts(maesn);
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("accountingRetrieveBankAccounts failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.GetBankAccountsRequest](../../models/operations/get-bank-accounts-request.md)                                                                                      | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.GetBankAccountsResponse](../../models/operations/get-bank-accounts-response.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |

## addBankAccount

### Example Usage

<!-- UsageSnippet language="typescript" operationID="createBankAccount" method="post" path="/accounting/bankAccounts" -->
```typescript
import { Maesn } from "maesn";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
});

async function run() {
  const result = await maesn.accounting.addBankAccount({
    body: {
      balance: 703.54,
      bankName: "<value>",
      bic: "<value>",
      currency: "LAK",
      description: "despite summer unnecessarily often afterwards achieve sedately incandescence",
      fileType: "MT940",
      iban: "SA3080240431D1A282278275",
      name: "<value>",
      number: "<value>",
      system: "<value>",
      status: "ACTIVE",
      type: "NON_CURRENT_LIABILITY",
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
import { accountingAddBankAccount } from "maesn/funcs/accounting-add-bank-account.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
});

async function run() {
  const res = await accountingAddBankAccount(maesn, {
    body: {
      balance: 703.54,
      bankName: "<value>",
      bic: "<value>",
      currency: "LAK",
      description: "despite summer unnecessarily often afterwards achieve sedately incandescence",
      fileType: "MT940",
      iban: "SA3080240431D1A282278275",
      name: "<value>",
      number: "<value>",
      system: "<value>",
      status: "ACTIVE",
      type: "NON_CURRENT_LIABILITY",
    },
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("accountingAddBankAccount failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.CreateBankAccountRequest](../../models/operations/create-bank-account-request.md)                                                                                  | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.CreateBankAccountResponse](../../models/operations/create-bank-account-response.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |

## fetchBankAccount

### Example Usage

<!-- UsageSnippet language="typescript" operationID="getBankAccount" method="get" path="/accounting/bankAccounts/{bankAccountId}" -->
```typescript
import { Maesn } from "maesn";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
});

async function run() {
  const result = await maesn.accounting.fetchBankAccount({
    bankAccountId: "<id>",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { MaesnCore } from "maesn/core.js";
import { accountingFetchBankAccount } from "maesn/funcs/accounting-fetch-bank-account.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
});

async function run() {
  const res = await accountingFetchBankAccount(maesn, {
    bankAccountId: "<id>",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("accountingFetchBankAccount failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.GetBankAccountRequest](../../models/operations/get-bank-account-request.md)                                                                                        | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.GetBankAccountResponse](../../models/operations/get-bank-account-response.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |

## retrieveDimensions

### Example Usage

<!-- UsageSnippet language="typescript" operationID="getDimensions" method="get" path="/accounting/dimensions" -->
```typescript
import { Maesn } from "maesn";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
});

async function run() {
  const result = await maesn.accounting.retrieveDimensions();

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { MaesnCore } from "maesn/core.js";
import { accountingRetrieveDimensions } from "maesn/funcs/accounting-retrieve-dimensions.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
});

async function run() {
  const res = await accountingRetrieveDimensions(maesn);
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("accountingRetrieveDimensions failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.GetDimensionsRequest](../../models/operations/get-dimensions-request.md)                                                                                           | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.GetDimensionsResponse](../../models/operations/get-dimensions-response.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |

## recordTransaction

### Example Usage

<!-- UsageSnippet language="typescript" operationID="createTransaction" method="post" path="/accounting/transactions" -->
```typescript
import { Maesn } from "maesn";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
});

async function run() {
  const result = await maesn.accounting.recordTransaction({
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
import { accountingRecordTransaction } from "maesn/funcs/accounting-record-transaction.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
});

async function run() {
  const res = await accountingRecordTransaction(maesn, {
    body: {},
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("accountingRecordTransaction failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.CreateTransactionRequest](../../models/operations/create-transaction-request.md)                                                                                   | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.CreateTransactionResponse](../../models/operations/create-transaction-response.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |

## fetchCustomers

### Example Usage

<!-- UsageSnippet language="typescript" operationID="getCustomers" method="get" path="/accounting/customers" -->
```typescript
import { Maesn } from "maesn";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
});

async function run() {
  const result = await maesn.accounting.fetchCustomers();

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { MaesnCore } from "maesn/core.js";
import { accountingFetchCustomers } from "maesn/funcs/accounting-fetch-customers.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
});

async function run() {
  const res = await accountingFetchCustomers(maesn);
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("accountingFetchCustomers failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.GetCustomersRequest](../../models/operations/get-customers-request.md)                                                                                             | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.GetCustomersResponse](../../models/operations/get-customers-response.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |

## createCustomer

### Example Usage

<!-- UsageSnippet language="typescript" operationID="createCustomer" method="post" path="/accounting/customers" -->
```typescript
import { Maesn } from "maesn";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
});

async function run() {
  const result = await maesn.accounting.createCustomer({
    body: {
      addresses: [],
      bankAccount: {
        bic: "<value>",
        holder: "<value>",
        isMainAccount: true,
        iban: "LU25377862T61M723A97",
        name: "<value>",
        sepa: true,
      },
      companyName: "Lind - Balistreri",
      contactPersons: [
        {
          emailAddresses: [],
          firstName: "Laurianne",
          lastName: "Blick",
          phoneNumbers: [
            "<value 1>",
          ],
          salutation: "<value>",
        },
      ],
      contactType: "CONTACT_PERSON",
      documentId: "<id>",
      emailAddresses: [
        {
          email: "Reymundo17@yahoo.com",
          type: "INVOICE",
        },
      ],
      number: "<value>",
      phoneNumbers: [],
      projectId: "<id>",
      role: "CONTACT",
      vatId: "<id>",
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
import { accountingCreateCustomer } from "maesn/funcs/accounting-create-customer.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
});

async function run() {
  const res = await accountingCreateCustomer(maesn, {
    body: {
      addresses: [],
      bankAccount: {
        bic: "<value>",
        holder: "<value>",
        isMainAccount: true,
        iban: "LU25377862T61M723A97",
        name: "<value>",
        sepa: true,
      },
      companyName: "Lind - Balistreri",
      contactPersons: [
        {
          emailAddresses: [],
          firstName: "Laurianne",
          lastName: "Blick",
          phoneNumbers: [
            "<value 1>",
          ],
          salutation: "<value>",
        },
      ],
      contactType: "CONTACT_PERSON",
      documentId: "<id>",
      emailAddresses: [
        {
          email: "Reymundo17@yahoo.com",
          type: "INVOICE",
        },
      ],
      number: "<value>",
      phoneNumbers: [],
      projectId: "<id>",
      role: "CONTACT",
      vatId: "<id>",
    },
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("accountingCreateCustomer failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.CreateCustomerRequest](../../models/operations/create-customer-request.md)                                                                                         | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.CreateCustomerResponse](../../models/operations/create-customer-response.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |

## fetchCustomer

### Example Usage

<!-- UsageSnippet language="typescript" operationID="getCustomer" method="get" path="/accounting/customers/{contactId}" -->
```typescript
import { Maesn } from "maesn";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
});

async function run() {
  const result = await maesn.accounting.fetchCustomer({
    contactId: "<id>",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { MaesnCore } from "maesn/core.js";
import { accountingFetchCustomer } from "maesn/funcs/accounting-fetch-customer.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
});

async function run() {
  const res = await accountingFetchCustomer(maesn, {
    contactId: "<id>",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("accountingFetchCustomer failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.GetCustomerRequest](../../models/operations/get-customer-request.md)                                                                                               | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.GetCustomerResponse](../../models/operations/get-customer-response.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |

## updateCustomer

### Example Usage

<!-- UsageSnippet language="typescript" operationID="updateCustomer" method="put" path="/accounting/customers/{contactId}" -->
```typescript
import { Maesn } from "maesn";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
});

async function run() {
  const result = await maesn.accounting.updateCustomer({
    contactId: "<id>",
    body: {
      addresses: [],
      bankAccount: {
        bic: "<value>",
        holder: "<value>",
        isMainAccount: true,
        iban: "AT163702108702070797",
        name: "<value>",
        sepa: true,
      },
      companyName: "Murphy, Hirthe and Cruickshank",
      contactPersons: [],
      contactType: "COMPANY",
      documentId: "<id>",
      emailAddresses: [],
      number: "<value>",
      phoneNumbers: [
        {
          number: "<value>",
          type: "SKYPE",
        },
      ],
      projectId: "<id>",
      role: "CONTACT",
      vatId: "<id>",
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
import { accountingUpdateCustomer } from "maesn/funcs/accounting-update-customer.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
});

async function run() {
  const res = await accountingUpdateCustomer(maesn, {
    contactId: "<id>",
    body: {
      addresses: [],
      bankAccount: {
        bic: "<value>",
        holder: "<value>",
        isMainAccount: true,
        iban: "AT163702108702070797",
        name: "<value>",
        sepa: true,
      },
      companyName: "Murphy, Hirthe and Cruickshank",
      contactPersons: [],
      contactType: "COMPANY",
      documentId: "<id>",
      emailAddresses: [],
      number: "<value>",
      phoneNumbers: [
        {
          number: "<value>",
          type: "SKYPE",
        },
      ],
      projectId: "<id>",
      role: "CONTACT",
      vatId: "<id>",
    },
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("accountingUpdateCustomer failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.UpdateCustomerRequest](../../models/operations/update-customer-request.md)                                                                                         | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.UpdateCustomerResponse](../../models/operations/update-customer-response.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |

## amendCustomer

### Example Usage

<!-- UsageSnippet language="typescript" operationID="patchCustomers" method="patch" path="/accounting/customers/{contactId}" -->
```typescript
import { Maesn } from "maesn";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
});

async function run() {
  const result = await maesn.accounting.amendCustomer({
    contactId: "<id>",
    body: {
      contactType: "CONTACT_PERSON",
      companyName: "Lockman, Koch and Reilly",
      contactPersons: [
        {
          emailAddresses: [],
          firstName: "Louisa",
          lastName: "McGlynn",
          phoneNumbers: [
            "<value 1>",
            "<value 2>",
            "<value 3>",
          ],
          salutation: "<value>",
        },
      ],
      addresses: [
        {
          addressLine1: "69361 Aspen Close",
          addressLine2: "-",
          city: "Paramount",
          countryCode: "TK",
          postalCode: "90632-7148",
          type: "PICKUP",
        },
      ],
      emailAddresses: [
        {
          email: "Grady99@hotmail.com",
          type: "OFFICE",
        },
      ],
      phoneNumbers: [
        {
          number: "<value>",
          type: "MOBILE",
        },
      ],
      bankAccount: {
        iban: "BG90LETP01786613716608",
        bic: "<value>",
        holder: "<value>",
        sepa: true,
      },
      projectId: "<id>",
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
import { accountingAmendCustomer } from "maesn/funcs/accounting-amend-customer.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
});

async function run() {
  const res = await accountingAmendCustomer(maesn, {
    contactId: "<id>",
    body: {
      contactType: "CONTACT_PERSON",
      companyName: "Lockman, Koch and Reilly",
      contactPersons: [
        {
          emailAddresses: [],
          firstName: "Louisa",
          lastName: "McGlynn",
          phoneNumbers: [
            "<value 1>",
            "<value 2>",
            "<value 3>",
          ],
          salutation: "<value>",
        },
      ],
      addresses: [
        {
          addressLine1: "69361 Aspen Close",
          addressLine2: "-",
          city: "Paramount",
          countryCode: "TK",
          postalCode: "90632-7148",
          type: "PICKUP",
        },
      ],
      emailAddresses: [
        {
          email: "Grady99@hotmail.com",
          type: "OFFICE",
        },
      ],
      phoneNumbers: [
        {
          number: "<value>",
          type: "MOBILE",
        },
      ],
      bankAccount: {
        iban: "BG90LETP01786613716608",
        bic: "<value>",
        holder: "<value>",
        sepa: true,
      },
      projectId: "<id>",
    },
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("accountingAmendCustomer failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.PatchCustomersRequest](../../models/operations/patch-customers-request.md)                                                                                         | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.PatchCustomersResponse](../../models/operations/patch-customers-response.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |

## retrieveSuppliers

### Example Usage

<!-- UsageSnippet language="typescript" operationID="getSuppliers" method="get" path="/accounting/suppliers" -->
```typescript
import { Maesn } from "maesn";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
});

async function run() {
  const result = await maesn.accounting.retrieveSuppliers();

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { MaesnCore } from "maesn/core.js";
import { accountingRetrieveSuppliers } from "maesn/funcs/accounting-retrieve-suppliers.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
});

async function run() {
  const res = await accountingRetrieveSuppliers(maesn);
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("accountingRetrieveSuppliers failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.GetSuppliersRequest](../../models/operations/get-suppliers-request.md)                                                                                             | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.GetSuppliersResponse](../../models/operations/get-suppliers-response.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |

## addSupplier

### Example Usage

<!-- UsageSnippet language="typescript" operationID="createSupplier" method="post" path="/accounting/suppliers" -->
```typescript
import { Maesn } from "maesn";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
});

async function run() {
  const result = await maesn.accounting.addSupplier({
    body: {
      addresses: [
        {
          addressLine1: "6302 Central Avenue",
          addressLine2: "-",
          city: "New Madisen",
          countryCode: "IE",
          postalCode: "37621-1977",
          type: "WORK",
        },
      ],
      bankAccount: {
        bic: "<value>",
        holder: "<value>",
        isMainAccount: true,
        iban: "IS405661803400080880010020",
        name: "<value>",
        sepa: false,
      },
      companyName: "Murphy LLC",
      contactPersons: [],
      contactType: "COMPANY",
      documentId: "<id>",
      emailAddresses: [],
      number: "<value>",
      phoneNumbers: [
        {
          number: "<value>",
          type: "SKYPE",
        },
      ],
      projectId: "<id>",
      role: "SUPPLIER",
      vatId: "<id>",
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
import { accountingAddSupplier } from "maesn/funcs/accounting-add-supplier.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
});

async function run() {
  const res = await accountingAddSupplier(maesn, {
    body: {
      addresses: [
        {
          addressLine1: "6302 Central Avenue",
          addressLine2: "-",
          city: "New Madisen",
          countryCode: "IE",
          postalCode: "37621-1977",
          type: "WORK",
        },
      ],
      bankAccount: {
        bic: "<value>",
        holder: "<value>",
        isMainAccount: true,
        iban: "IS405661803400080880010020",
        name: "<value>",
        sepa: false,
      },
      companyName: "Murphy LLC",
      contactPersons: [],
      contactType: "COMPANY",
      documentId: "<id>",
      emailAddresses: [],
      number: "<value>",
      phoneNumbers: [
        {
          number: "<value>",
          type: "SKYPE",
        },
      ],
      projectId: "<id>",
      role: "SUPPLIER",
      vatId: "<id>",
    },
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("accountingAddSupplier failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.CreateSupplierRequest](../../models/operations/create-supplier-request.md)                                                                                         | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.CreateSupplierResponse](../../models/operations/create-supplier-response.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |

## fetchSupplier

### Example Usage

<!-- UsageSnippet language="typescript" operationID="getSupplier" method="get" path="/accounting/suppliers/{contactId}" -->
```typescript
import { Maesn } from "maesn";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
});

async function run() {
  const result = await maesn.accounting.fetchSupplier({
    contactId: "<id>",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { MaesnCore } from "maesn/core.js";
import { accountingFetchSupplier } from "maesn/funcs/accounting-fetch-supplier.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
});

async function run() {
  const res = await accountingFetchSupplier(maesn, {
    contactId: "<id>",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("accountingFetchSupplier failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.GetSupplierRequest](../../models/operations/get-supplier-request.md)                                                                                               | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.GetSupplierResponse](../../models/operations/get-supplier-response.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |

## modifySupplier

### Example Usage

<!-- UsageSnippet language="typescript" operationID="updateSupplier" method="put" path="/accounting/suppliers/{contactId}" -->
```typescript
import { Maesn } from "maesn";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
});

async function run() {
  const result = await maesn.accounting.modifySupplier({
    contactId: "<id>",
    body: {
      addresses: [
        {
          addressLine1: "7522 Bins Avenue",
          addressLine2: "-",
          city: "National City",
          countryCode: "RS",
          postalCode: "22514-2574",
          type: "BILLING",
        },
      ],
      bankAccount: {
        bic: "<value>",
        holder: "<value>",
        isMainAccount: true,
        iban: "TL140693001201006031557",
        name: "<value>",
        sepa: true,
      },
      companyName: "Bergnaum Inc",
      contactPersons: [],
      contactType: "CONTACT_PERSON",
      documentId: "<id>",
      emailAddresses: [
        {
          email: "Camille_Nader@hotmail.com",
          type: "PRIVATE",
        },
      ],
      number: "<value>",
      phoneNumbers: [],
      projectId: "<id>",
      role: "CUSTOMER",
      vatId: "<id>",
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
import { accountingModifySupplier } from "maesn/funcs/accounting-modify-supplier.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
});

async function run() {
  const res = await accountingModifySupplier(maesn, {
    contactId: "<id>",
    body: {
      addresses: [
        {
          addressLine1: "7522 Bins Avenue",
          addressLine2: "-",
          city: "National City",
          countryCode: "RS",
          postalCode: "22514-2574",
          type: "BILLING",
        },
      ],
      bankAccount: {
        bic: "<value>",
        holder: "<value>",
        isMainAccount: true,
        iban: "TL140693001201006031557",
        name: "<value>",
        sepa: true,
      },
      companyName: "Bergnaum Inc",
      contactPersons: [],
      contactType: "CONTACT_PERSON",
      documentId: "<id>",
      emailAddresses: [
        {
          email: "Camille_Nader@hotmail.com",
          type: "PRIVATE",
        },
      ],
      number: "<value>",
      phoneNumbers: [],
      projectId: "<id>",
      role: "CUSTOMER",
      vatId: "<id>",
    },
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("accountingModifySupplier failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.UpdateSupplierRequest](../../models/operations/update-supplier-request.md)                                                                                         | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.UpdateSupplierResponse](../../models/operations/update-supplier-response.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |

## amendSupplier

### Example Usage

<!-- UsageSnippet language="typescript" operationID="patchSupplier" method="patch" path="/accounting/suppliers/{contactId}" -->
```typescript
import { Maesn } from "maesn";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
});

async function run() {
  const result = await maesn.accounting.amendSupplier({
    contactId: "<id>",
    body: {
      contactType: "COMPANY",
      companyName: "Lehner Group",
      contactPersons: [
        {
          emailAddresses: [],
          firstName: "Jean",
          lastName: "Stiedemann",
          phoneNumbers: [
            "<value 1>",
          ],
          salutation: "<value>",
        },
      ],
      addresses: [],
      emailAddresses: [],
      phoneNumbers: [],
      bankAccount: {
        iban: "BH09HZUG8597921H253895",
        bic: "<value>",
        holder: "<value>",
        sepa: false,
      },
      projectId: "<id>",
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
import { accountingAmendSupplier } from "maesn/funcs/accounting-amend-supplier.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
});

async function run() {
  const res = await accountingAmendSupplier(maesn, {
    contactId: "<id>",
    body: {
      contactType: "COMPANY",
      companyName: "Lehner Group",
      contactPersons: [
        {
          emailAddresses: [],
          firstName: "Jean",
          lastName: "Stiedemann",
          phoneNumbers: [
            "<value 1>",
          ],
          salutation: "<value>",
        },
      ],
      addresses: [],
      emailAddresses: [],
      phoneNumbers: [],
      bankAccount: {
        iban: "BH09HZUG8597921H253895",
        bic: "<value>",
        holder: "<value>",
        sepa: false,
      },
      projectId: "<id>",
    },
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("accountingAmendSupplier failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.PatchSupplierRequest](../../models/operations/patch-supplier-request.md)                                                                                           | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.PatchSupplierResponse](../../models/operations/patch-supplier-response.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |

## getContacts

### Example Usage

<!-- UsageSnippet language="typescript" operationID="getContacts" method="get" path="/accounting/contacts" -->
```typescript
import { Maesn } from "maesn";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
});

async function run() {
  const result = await maesn.accounting.getContacts();

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { MaesnCore } from "maesn/core.js";
import { accountingGetContacts } from "maesn/funcs/accounting-get-contacts.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
});

async function run() {
  const res = await accountingGetContacts(maesn);
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("accountingGetContacts failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.GetContactsRequest](../../models/operations/get-contacts-request.md)                                                                                               | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.GetContactsResponse](../../models/operations/get-contacts-response.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |

## addContact

### Example Usage

<!-- UsageSnippet language="typescript" operationID="createContact" method="post" path="/accounting/contacts" -->
```typescript
import { Maesn } from "maesn";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
});

async function run() {
  const result = await maesn.accounting.addContact({
    body: {
      id: "<id>",
      addresses: [],
      companyName: "Kessler and Sons",
      contactPersons: [],
      contactType: "COMPANY",
      emailAddresses: [
        {
          email: "Lawrence31@gmail.com",
          type: "INVOICE",
        },
      ],
      isCustomer: true,
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
import { accountingAddContact } from "maesn/funcs/accounting-add-contact.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
});

async function run() {
  const res = await accountingAddContact(maesn, {
    body: {
      id: "<id>",
      addresses: [],
      companyName: "Kessler and Sons",
      contactPersons: [],
      contactType: "COMPANY",
      emailAddresses: [
        {
          email: "Lawrence31@gmail.com",
          type: "INVOICE",
        },
      ],
      isCustomer: true,
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
    console.log("accountingAddContact failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.CreateContactRequest](../../models/operations/create-contact-request.md)                                                                                           | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.CreateContactResponse](../../models/operations/create-contact-response.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |

## fetchContact

### Example Usage

<!-- UsageSnippet language="typescript" operationID="getContact" method="get" path="/accounting/contacts/{contactId}" -->
```typescript
import { Maesn } from "maesn";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
});

async function run() {
  const result = await maesn.accounting.fetchContact({
    contactId: "<id>",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { MaesnCore } from "maesn/core.js";
import { accountingFetchContact } from "maesn/funcs/accounting-fetch-contact.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
});

async function run() {
  const res = await accountingFetchContact(maesn, {
    contactId: "<id>",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("accountingFetchContact failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.GetContactRequest](../../models/operations/get-contact-request.md)                                                                                                 | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.GetContactResponse](../../models/operations/get-contact-response.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |

## replaceContact

### Example Usage

<!-- UsageSnippet language="typescript" operationID="putContact" method="put" path="/accounting/contacts/{contactId}" -->
```typescript
import { Maesn } from "maesn";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
});

async function run() {
  const result = await maesn.accounting.replaceContact({
    contactId: "<id>",
    body: {
      id: "<id>",
      addresses: [],
      companyName: "Rolfson - Gerlach",
      contactPersons: [],
      contactType: "COMPANY",
      emailAddresses: [
        {
          email: "Sunny.Koch@gmail.com",
          type: "OTHER",
        },
      ],
      isCustomer: true,
      isSupplier: false,
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
import { accountingReplaceContact } from "maesn/funcs/accounting-replace-contact.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
});

async function run() {
  const res = await accountingReplaceContact(maesn, {
    contactId: "<id>",
    body: {
      id: "<id>",
      addresses: [],
      companyName: "Rolfson - Gerlach",
      contactPersons: [],
      contactType: "COMPANY",
      emailAddresses: [
        {
          email: "Sunny.Koch@gmail.com",
          type: "OTHER",
        },
      ],
      isCustomer: true,
      isSupplier: false,
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
    console.log("accountingReplaceContact failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.PutContactRequest](../../models/operations/put-contact-request.md)                                                                                                 | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.PutContactResponse](../../models/operations/put-contact-response.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |

## createContactsBulk

### Example Usage

<!-- UsageSnippet language="typescript" operationID="createContacts" method="post" path="/accounting/contacts/bulk" -->
```typescript
import { Maesn } from "maesn";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
});

async function run() {
  const result = await maesn.accounting.createContactsBulk({
    body: {
      accountNumberLength: 8670.85,
      chartOfAccount: "SKR03",
      entries: [
        {
          id: "<id>",
          addresses: [
            {
              addressLine1: "32634 Berniece Club",
              addressLine2: "-",
              city: "Tyler",
              countryCode: "MA",
              postalCode: "16147-7872",
              type: "PICKUP",
            },
          ],
          companyName: "Kessler LLC",
          contactPersons: [
            {
              id: "<id>",
              emailAddresses: [],
              firstName: "Leonor",
              lastName: "Jones",
              phoneNumbers: [
                {
                  number: "<value>",
                  type: "MOBILE",
                },
              ],
              salutation: "<value>",
            },
          ],
          contactType: "CONTACT_PERSON",
          emailAddresses: [
            {
              email: "Ivory.Corwin35@yahoo.com",
              type: "PAYMENT",
            },
          ],
          isCustomer: false,
          isSupplier: true,
          number: "<value>",
          phoneNumbers: [
            {
              number: "<value>",
              type: "MOBILE",
            },
          ],
          projectId: "<id>",
          website: "<value>",
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
import { accountingCreateContactsBulk } from "maesn/funcs/accounting-create-contacts-bulk.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
});

async function run() {
  const res = await accountingCreateContactsBulk(maesn, {
    body: {
      accountNumberLength: 8670.85,
      chartOfAccount: "SKR03",
      entries: [
        {
          id: "<id>",
          addresses: [
            {
              addressLine1: "32634 Berniece Club",
              addressLine2: "-",
              city: "Tyler",
              countryCode: "MA",
              postalCode: "16147-7872",
              type: "PICKUP",
            },
          ],
          companyName: "Kessler LLC",
          contactPersons: [
            {
              id: "<id>",
              emailAddresses: [],
              firstName: "Leonor",
              lastName: "Jones",
              phoneNumbers: [
                {
                  number: "<value>",
                  type: "MOBILE",
                },
              ],
              salutation: "<value>",
            },
          ],
          contactType: "CONTACT_PERSON",
          emailAddresses: [
            {
              email: "Ivory.Corwin35@yahoo.com",
              type: "PAYMENT",
            },
          ],
          isCustomer: false,
          isSupplier: true,
          number: "<value>",
          phoneNumbers: [
            {
              number: "<value>",
              type: "MOBILE",
            },
          ],
          projectId: "<id>",
          website: "<value>",
        },
      ],
      fiscalYearStartDate: "<value>",
    },
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("accountingCreateContactsBulk failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.CreateContactsRequest](../../models/operations/create-contacts-request.md)                                                                                         | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.CreateContactsResponse](../../models/operations/create-contacts-response.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |

## batchAddContacts

### Example Usage

<!-- UsageSnippet language="typescript" operationID="createContactsV1" method="post" path="/accounting/batch/contacts" -->
```typescript
import { Maesn } from "maesn";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
});

async function run() {
  const result = await maesn.accounting.batchAddContacts({
    body: {
      accountNumberLength: 3935.59,
      chartOfAccount: "SKR51",
      entries: [],
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
import { accountingBatchAddContacts } from "maesn/funcs/accounting-batch-add-contacts.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
});

async function run() {
  const res = await accountingBatchAddContacts(maesn, {
    body: {
      accountNumberLength: 3935.59,
      chartOfAccount: "SKR51",
      entries: [],
      fiscalYearStartDate: "<value>",
    },
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("accountingBatchAddContacts failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.CreateContactsV1Request](../../models/operations/create-contacts-v1-request.md)                                                                                    | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.CreateContactsV1Response](../../models/operations/create-contacts-v1-response.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |

## retrieveInvoices

### Example Usage

<!-- UsageSnippet language="typescript" operationID="getInvoices" method="get" path="/accounting/invoices" -->
```typescript
import { Maesn } from "maesn";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
});

async function run() {
  const result = await maesn.accounting.retrieveInvoices();

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { MaesnCore } from "maesn/core.js";
import { accountingRetrieveInvoices } from "maesn/funcs/accounting-retrieve-invoices.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
});

async function run() {
  const res = await accountingRetrieveInvoices(maesn);
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("accountingRetrieveInvoices failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.GetInvoicesRequest](../../models/operations/get-invoices-request.md)                                                                                               | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.GetInvoicesResponse](../../models/operations/get-invoices-response.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |

## addInvoice

### Example Usage

<!-- UsageSnippet language="typescript" operationID="createInvoice" method="post" path="/accounting/invoices" -->
```typescript
import { Maesn } from "maesn";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
});

async function run() {
  const result = await maesn.accounting.addInvoice({
    body: {
      invoiceId: "<id>",
      addresses: [
        {
          addressLine1: "42975 Haleigh Flat",
          addressLine2: "-",
          city: "North Kaseycester",
          countryCode: "KG",
          postalCode: "18386-8735",
          type: "DELIVERY",
        },
      ],
      contactId: "<id>",
      currency: "Iceland Krona",
      discountPercentage: 3686.22,
      dueDate: "<value>",
      fileId: "<id>",
      grossTotalAmount: 2774.64,
      invoiceDate: "<value>",
      invoiceNumber: "<value>",
      invoiceType: "BILL",
      journalCode: "<value>",
      lineAmountTypes: "<value>",
      lineItems: [],
      name: "<value>",
      oneLineAddress: "<value>",
      paidDate: "<value>",
      paymentTermDuration: 3652.63,
      paymentTermId: "<id>",
      reference: "<value>",
      shippingDate: "<value>",
      shippingType: "NONE",
      shippingEndDate: "<value>",
      status: "PARTIALLY_PAID",
      taxRule: "NET",
      taxText: "<value>",
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
import { accountingAddInvoice } from "maesn/funcs/accounting-add-invoice.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
});

async function run() {
  const res = await accountingAddInvoice(maesn, {
    body: {
      invoiceId: "<id>",
      addresses: [
        {
          addressLine1: "42975 Haleigh Flat",
          addressLine2: "-",
          city: "North Kaseycester",
          countryCode: "KG",
          postalCode: "18386-8735",
          type: "DELIVERY",
        },
      ],
      contactId: "<id>",
      currency: "Iceland Krona",
      discountPercentage: 3686.22,
      dueDate: "<value>",
      fileId: "<id>",
      grossTotalAmount: 2774.64,
      invoiceDate: "<value>",
      invoiceNumber: "<value>",
      invoiceType: "BILL",
      journalCode: "<value>",
      lineAmountTypes: "<value>",
      lineItems: [],
      name: "<value>",
      oneLineAddress: "<value>",
      paidDate: "<value>",
      paymentTermDuration: 3652.63,
      paymentTermId: "<id>",
      reference: "<value>",
      shippingDate: "<value>",
      shippingType: "NONE",
      shippingEndDate: "<value>",
      status: "PARTIALLY_PAID",
      taxRule: "NET",
      taxText: "<value>",
    },
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("accountingAddInvoice failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.CreateInvoiceRequest](../../models/operations/create-invoice-request.md)                                                                                           | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.CreateInvoiceResponse](../../models/operations/create-invoice-response.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |

## fetchInvoice

### Example Usage

<!-- UsageSnippet language="typescript" operationID="getInvoice" method="get" path="/accounting/invoices/{invoiceId}" -->
```typescript
import { Maesn } from "maesn";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
});

async function run() {
  const result = await maesn.accounting.fetchInvoice({
    invoiceId: "<id>",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { MaesnCore } from "maesn/core.js";
import { accountingFetchInvoice } from "maesn/funcs/accounting-fetch-invoice.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
});

async function run() {
  const res = await accountingFetchInvoice(maesn, {
    invoiceId: "<id>",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("accountingFetchInvoice failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.GetInvoiceRequest](../../models/operations/get-invoice-request.md)                                                                                                 | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.GetInvoiceResponse](../../models/operations/get-invoice-response.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |

## amendInvoice

### Example Usage

<!-- UsageSnippet language="typescript" operationID="patchInvoice" method="patch" path="/accounting/invoices/{invoiceId}" -->
```typescript
import { Maesn } from "maesn";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
});

async function run() {
  const result = await maesn.accounting.amendInvoice({
    invoiceId: "<id>",
    body: {
      invoiceId: "<id>",
      contactId: "<id>",
      name: "<value>",
      reference: "<value>",
      currency: "Canadian Dollar",
      invoiceDate: "<value>",
      journalCode: "<value>",
      paymentTermId: "<id>",
      fileId: "<id>",
      status: "PARTIALLY_PAID",
      invoiceType: "BILL",
      oneLineAddress: "<value>",
      addresses: [],
      taxRule: "DEFAULT",
      taxText: "<value>",
      lineItems: [],
      discountPercentage: 225.27,
      shippingType: "SERVICEPERIOD",
      shippingDate: "<value>",
      shippingEndDate: "<value>",
      lineAmountTypes: "NOTAX",
      dueDate: "<value>",
      paidDate: "<value>",
      paymentTermDuration: 6916.25,
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
import { accountingAmendInvoice } from "maesn/funcs/accounting-amend-invoice.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
});

async function run() {
  const res = await accountingAmendInvoice(maesn, {
    invoiceId: "<id>",
    body: {
      invoiceId: "<id>",
      contactId: "<id>",
      name: "<value>",
      reference: "<value>",
      currency: "Canadian Dollar",
      invoiceDate: "<value>",
      journalCode: "<value>",
      paymentTermId: "<id>",
      fileId: "<id>",
      status: "PARTIALLY_PAID",
      invoiceType: "BILL",
      oneLineAddress: "<value>",
      addresses: [],
      taxRule: "DEFAULT",
      taxText: "<value>",
      lineItems: [],
      discountPercentage: 225.27,
      shippingType: "SERVICEPERIOD",
      shippingDate: "<value>",
      shippingEndDate: "<value>",
      lineAmountTypes: "NOTAX",
      dueDate: "<value>",
      paidDate: "<value>",
      paymentTermDuration: 6916.25,
    },
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("accountingAmendInvoice failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.PatchInvoiceRequest](../../models/operations/patch-invoice-request.md)                                                                                             | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.PatchInvoiceResponse](../../models/operations/patch-invoice-response.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |

## fetchInvoiceDocument

### Example Usage

<!-- UsageSnippet language="typescript" operationID="getInvoiceDocument" method="get" path="/accounting/invoices/{invoiceId}/document" -->
```typescript
import { Maesn } from "maesn";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
});

async function run() {
  const result = await maesn.accounting.fetchInvoiceDocument({
    invoiceId: "<id>",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { MaesnCore } from "maesn/core.js";
import { accountingFetchInvoiceDocument } from "maesn/funcs/accounting-fetch-invoice-document.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
});

async function run() {
  const res = await accountingFetchInvoiceDocument(maesn, {
    invoiceId: "<id>",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("accountingFetchInvoiceDocument failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.GetInvoiceDocumentRequest](../../models/operations/get-invoice-document-request.md)                                                                                | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.GetInvoiceDocumentResponse](../../models/operations/get-invoice-document-response.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |

## uploadFile

### Example Usage

<!-- UsageSnippet language="typescript" operationID="postFile" method="post" path="/accounting/files" -->
```typescript
import { Maesn } from "maesn";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
});

async function run() {
  const result = await maesn.accounting.uploadFile({
    body: {
      contactId: "Contact id associated to the document",
      documentDate: "2025-03-26T08:25:54.060Z",
      documentId: "b5e624e5-fb9e-4836-a443-87a3820f5b48",
      documentType: "Rechnungsausgang",
      integrationSource: "3rd party app",
      note: "note for the document",
      resourceId: "Id of the reference object (bill or invoice id).",
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
import { accountingUploadFile } from "maesn/funcs/accounting-upload-file.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
});

async function run() {
  const res = await accountingUploadFile(maesn, {
    body: {
      contactId: "Contact id associated to the document",
      documentDate: "2025-03-26T08:25:54.060Z",
      documentId: "b5e624e5-fb9e-4836-a443-87a3820f5b48",
      documentType: "Rechnungsausgang",
      integrationSource: "3rd party app",
      note: "note for the document",
      resourceId: "Id of the reference object (bill or invoice id).",
    },
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("accountingUploadFile failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.PostFileRequest](../../models/operations/post-file-request.md)                                                                                                     | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.PostFileResponse](../../models/operations/post-file-response.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |

## fetchDocumentTypes

### Example Usage

<!-- UsageSnippet language="typescript" operationID="getDocumentTypes" method="get" path="/accounting/files/documentTypes" -->
```typescript
import { Maesn } from "maesn";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
});

async function run() {
  const result = await maesn.accounting.fetchDocumentTypes();

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { MaesnCore } from "maesn/core.js";
import { accountingFetchDocumentTypes } from "maesn/funcs/accounting-fetch-document-types.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
});

async function run() {
  const res = await accountingFetchDocumentTypes(maesn);
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("accountingFetchDocumentTypes failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.GetDocumentTypesRequest](../../models/operations/get-document-types-request.md)                                                                                    | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.GetDocumentTypesResponse](../../models/operations/get-document-types-response.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |

## getAsyncTask

### Example Usage

<!-- UsageSnippet language="typescript" operationID="getAsyncTaskInfo" method="get" path="/accounting/asyncTask/{taskId}" -->
```typescript
import { Maesn } from "maesn";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
});

async function run() {
  const result = await maesn.accounting.getAsyncTask({
    taskId: "<id>",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { MaesnCore } from "maesn/core.js";
import { accountingGetAsyncTask } from "maesn/funcs/accounting-get-async-task.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
});

async function run() {
  const res = await accountingGetAsyncTask(maesn, {
    taskId: "<id>",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("accountingGetAsyncTask failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.GetAsyncTaskInfoRequest](../../models/operations/get-async-task-info-request.md)                                                                                   | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.GetAsyncTaskInfoResponse](../../models/operations/get-async-task-info-response.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |

## retrieveItems

### Example Usage

<!-- UsageSnippet language="typescript" operationID="getItems" method="get" path="/accounting/items" -->
```typescript
import { Maesn } from "maesn";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
});

async function run() {
  const result = await maesn.accounting.retrieveItems();

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { MaesnCore } from "maesn/core.js";
import { accountingRetrieveItems } from "maesn/funcs/accounting-retrieve-items.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
});

async function run() {
  const res = await accountingRetrieveItems(maesn);
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("accountingRetrieveItems failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.GetItemsRequest](../../models/operations/get-items-request.md)                                                                                                     | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.GetItemsResponse](../../models/operations/get-items-response.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |

## fetchItem

### Example Usage

<!-- UsageSnippet language="typescript" operationID="getItem" method="get" path="/accounting/items/{itemId}" -->
```typescript
import { Maesn } from "maesn";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
});

async function run() {
  const result = await maesn.accounting.fetchItem({
    itemId: "<id>",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { MaesnCore } from "maesn/core.js";
import { accountingFetchItem } from "maesn/funcs/accounting-fetch-item.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
});

async function run() {
  const res = await accountingFetchItem(maesn, {
    itemId: "<id>",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("accountingFetchItem failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.GetItemRequest](../../models/operations/get-item-request.md)                                                                                                       | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.GetItemResponse](../../models/operations/get-item-response.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |

## retrieveInvoiceLineItems

### Example Usage

<!-- UsageSnippet language="typescript" operationID="getLineItems" method="get" path="/accounting/invoices/{invoiceId}/lineItems" -->
```typescript
import { Maesn } from "maesn";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
});

async function run() {
  const result = await maesn.accounting.retrieveInvoiceLineItems({
    invoiceId: "<id>",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { MaesnCore } from "maesn/core.js";
import { accountingRetrieveInvoiceLineItems } from "maesn/funcs/accounting-retrieve-invoice-line-items.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
});

async function run() {
  const res = await accountingRetrieveInvoiceLineItems(maesn, {
    invoiceId: "<id>",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("accountingRetrieveInvoiceLineItems failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.GetLineItemsRequest](../../models/operations/get-line-items-request.md)                                                                                            | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.GetLineItemsResponse](../../models/operations/get-line-items-response.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |

## addInvoiceLineItem

### Example Usage

<!-- UsageSnippet language="typescript" operationID="createLineItem" method="post" path="/accounting/invoices/{invoiceId}/lineItems" -->
```typescript
import { Maesn } from "maesn";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
});

async function run() {
  const result = await maesn.accounting.addInvoiceLineItem({
    invoiceId: "<id>",
    body: {
      accountCode: "<value>",
      accountId: "<id>",
      description: "pluck wherever next magnificent ew millet for absent",
      dimensions: [
        {
          id: "<id>",
          categoryName: "<value>",
          name: "<value>",
        },
      ],
      discountItemPercentage: 9896.72,
      grossAmount: 356.93,
      itemId: "<id>",
      name: "<value>",
      quantity: 931.68,
      taxCode: "<value>",
      taxRatePercentage: 3707.03,
      taxType: "<value>",
      type: "<value>",
      unitAmount: 1361.58,
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
import { accountingAddInvoiceLineItem } from "maesn/funcs/accounting-add-invoice-line-item.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
});

async function run() {
  const res = await accountingAddInvoiceLineItem(maesn, {
    invoiceId: "<id>",
    body: {
      accountCode: "<value>",
      accountId: "<id>",
      description: "pluck wherever next magnificent ew millet for absent",
      dimensions: [
        {
          id: "<id>",
          categoryName: "<value>",
          name: "<value>",
        },
      ],
      discountItemPercentage: 9896.72,
      grossAmount: 356.93,
      itemId: "<id>",
      name: "<value>",
      quantity: 931.68,
      taxCode: "<value>",
      taxRatePercentage: 3707.03,
      taxType: "<value>",
      type: "<value>",
      unitAmount: 1361.58,
      unitName: "<value>",
    },
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("accountingAddInvoiceLineItem failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.CreateLineItemRequest](../../models/operations/create-line-item-request.md)                                                                                        | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.CreateLineItemResponse](../../models/operations/create-line-item-response.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |

## retrieveInvoiceLineItem

### Example Usage

<!-- UsageSnippet language="typescript" operationID="getLineItem" method="get" path="/accounting/invoices/{invoiceId}/lineItems/{lineItemId}" -->
```typescript
import { Maesn } from "maesn";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
});

async function run() {
  const result = await maesn.accounting.retrieveInvoiceLineItem({
    invoiceId: "<id>",
    lineItemId: "<id>",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { MaesnCore } from "maesn/core.js";
import { accountingRetrieveInvoiceLineItem } from "maesn/funcs/accounting-retrieve-invoice-line-item.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
});

async function run() {
  const res = await accountingRetrieveInvoiceLineItem(maesn, {
    invoiceId: "<id>",
    lineItemId: "<id>",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("accountingRetrieveInvoiceLineItem failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.GetLineItemRequest](../../models/operations/get-line-item-request.md)                                                                                              | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.GetLineItemResponse](../../models/operations/get-line-item-response.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |

## fetchJournals

### Example Usage

<!-- UsageSnippet language="typescript" operationID="getJournals" method="get" path="/accounting/journals" -->
```typescript
import { Maesn } from "maesn";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
});

async function run() {
  const result = await maesn.accounting.fetchJournals();

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { MaesnCore } from "maesn/core.js";
import { accountingFetchJournals } from "maesn/funcs/accounting-fetch-journals.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
});

async function run() {
  const res = await accountingFetchJournals(maesn);
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("accountingFetchJournals failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.GetJournalsRequest](../../models/operations/get-journals-request.md)                                                                                               | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.GetJournalsResponse](../../models/operations/get-journals-response.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |

## listJournalEntries

### Example Usage

<!-- UsageSnippet language="typescript" operationID="getJournalEntries" method="get" path="/accounting/journalEntries" -->
```typescript
import { Maesn } from "maesn";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
});

async function run() {
  const result = await maesn.accounting.listJournalEntries();

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { MaesnCore } from "maesn/core.js";
import { accountingListJournalEntries } from "maesn/funcs/accounting-list-journal-entries.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
});

async function run() {
  const res = await accountingListJournalEntries(maesn);
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("accountingListJournalEntries failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.GetJournalEntriesRequest](../../models/operations/get-journal-entries-request.md)                                                                                  | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.GetJournalEntriesResponse](../../models/operations/get-journal-entries-response.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |

## addJournalEntry

### Example Usage

<!-- UsageSnippet language="typescript" operationID="createJournalEntry" method="post" path="/accounting/journalEntries" -->
```typescript
import { Maesn } from "maesn";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
});

async function run() {
  const result = await maesn.accounting.addJournalEntry({
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
import { accountingAddJournalEntry } from "maesn/funcs/accounting-add-journal-entry.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
});

async function run() {
  const res = await accountingAddJournalEntry(maesn, {
    body: {},
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("accountingAddJournalEntry failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.CreateJournalEntryRequest](../../models/operations/create-journal-entry-request.md)                                                                                | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.CreateJournalEntryResponse](../../models/operations/create-journal-entry-response.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |

## fetchJournalEntry

### Example Usage

<!-- UsageSnippet language="typescript" operationID="getJournalEntry" method="get" path="/accounting/journalEntries/{journalEntryId}" -->
```typescript
import { Maesn } from "maesn";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
});

async function run() {
  const result = await maesn.accounting.fetchJournalEntry({
    journalEntryId: "<id>",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { MaesnCore } from "maesn/core.js";
import { accountingFetchJournalEntry } from "maesn/funcs/accounting-fetch-journal-entry.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
});

async function run() {
  const res = await accountingFetchJournalEntry(maesn, {
    journalEntryId: "<id>",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("accountingFetchJournalEntry failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.GetJournalEntryRequest](../../models/operations/get-journal-entry-request.md)                                                                                      | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.GetJournalEntryResponse](../../models/operations/get-journal-entry-response.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |

## createJournalEntryAttachments

### Example Usage

<!-- UsageSnippet language="typescript" operationID="createJournalEntryAttachments" method="post" path="/accounting/journalEntries/{journalEntryId}/Attachments" -->
```typescript
import { Maesn } from "maesn";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
});

async function run() {
  const result = await maesn.accounting.createJournalEntryAttachments({
    journalEntryId: "<id>",
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
import { accountingCreateJournalEntryAttachments } from "maesn/funcs/accounting-create-journal-entry-attachments.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
});

async function run() {
  const res = await accountingCreateJournalEntryAttachments(maesn, {
    journalEntryId: "<id>",
    body: {},
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("accountingCreateJournalEntryAttachments failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.CreateJournalEntryAttachmentsRequest](../../models/operations/create-journal-entry-attachments-request.md)                                                         | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.CreateJournalEntryAttachmentsResponse](../../models/operations/create-journal-entry-attachments-response.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |

## fetchOffers

### Example Usage

<!-- UsageSnippet language="typescript" operationID="getOffers" method="get" path="/accounting/offers" -->
```typescript
import { Maesn } from "maesn";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
});

async function run() {
  const result = await maesn.accounting.fetchOffers();

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { MaesnCore } from "maesn/core.js";
import { accountingFetchOffers } from "maesn/funcs/accounting-fetch-offers.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
});

async function run() {
  const res = await accountingFetchOffers(maesn);
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("accountingFetchOffers failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.GetOffersRequest](../../models/operations/get-offers-request.md)                                                                                                   | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.GetOffersResponse](../../models/operations/get-offers-response.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |

## addOffer

### Example Usage

<!-- UsageSnippet language="typescript" operationID="createOffer" method="post" path="/accounting/offers" -->
```typescript
import { Maesn } from "maesn";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
});

async function run() {
  const result = await maesn.accounting.addOffer({
    body: {
      addresses: [
        {
          addressLine1: "914 Mann Ridge",
          addressLine2: "-",
          city: "Franeyshire",
          countryCode: "RS",
          postalCode: "73463",
          type: "SELLING",
        },
      ],
      contactId: "<id>",
      currency: "Ethiopian Birr",
      lineItems: [
        {
          accountCode: "<value>",
          accountId: "<id>",
          description: "helplessly towards clamor hmph aw fumigate and",
          itemId: "<id>",
          name: "<value>",
          quantity: 4545.56,
          taxCode: "<value>",
          taxRatePercentage: 1334.93,
          taxType: "<value>",
          type: "ITEM",
          totalDiscountAmount: 200.15,
          totalDiscountPercentage: 7823.01,
          totalGrossAmount: 9228.49,
          totalNetAmount: 996.84,
          totalTaxAmount: 8491.69,
          unitAmount: 1509.46,
          unitDiscountAmount: 5094.14,
          unitDiscountPercentage: 6160.87,
          unitName: "<value>",
        },
      ],
      name: "<value>",
      offerDate: "<value>",
      offerNumber: "<value>",
      oneLineAddress: "<value>",
      reference: "<value>",
      status: "EXPIRED",
      taxText: "<value>",
      totalDiscountAmount: 7097.98,
      totalDiscountPercentage: 4784.75,
      totalGrossAmount: 8705.35,
      totalNetAmount: 1871.27,
      totalTaxAmount: 9099.91,
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
import { accountingAddOffer } from "maesn/funcs/accounting-add-offer.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
});

async function run() {
  const res = await accountingAddOffer(maesn, {
    body: {
      addresses: [
        {
          addressLine1: "914 Mann Ridge",
          addressLine2: "-",
          city: "Franeyshire",
          countryCode: "RS",
          postalCode: "73463",
          type: "SELLING",
        },
      ],
      contactId: "<id>",
      currency: "Ethiopian Birr",
      lineItems: [
        {
          accountCode: "<value>",
          accountId: "<id>",
          description: "helplessly towards clamor hmph aw fumigate and",
          itemId: "<id>",
          name: "<value>",
          quantity: 4545.56,
          taxCode: "<value>",
          taxRatePercentage: 1334.93,
          taxType: "<value>",
          type: "ITEM",
          totalDiscountAmount: 200.15,
          totalDiscountPercentage: 7823.01,
          totalGrossAmount: 9228.49,
          totalNetAmount: 996.84,
          totalTaxAmount: 8491.69,
          unitAmount: 1509.46,
          unitDiscountAmount: 5094.14,
          unitDiscountPercentage: 6160.87,
          unitName: "<value>",
        },
      ],
      name: "<value>",
      offerDate: "<value>",
      offerNumber: "<value>",
      oneLineAddress: "<value>",
      reference: "<value>",
      status: "EXPIRED",
      taxText: "<value>",
      totalDiscountAmount: 7097.98,
      totalDiscountPercentage: 4784.75,
      totalGrossAmount: 8705.35,
      totalNetAmount: 1871.27,
      totalTaxAmount: 9099.91,
    },
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("accountingAddOffer failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.CreateOfferRequest](../../models/operations/create-offer-request.md)                                                                                               | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.CreateOfferResponse](../../models/operations/create-offer-response.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |

## fetchOffer

### Example Usage

<!-- UsageSnippet language="typescript" operationID="getOffer" method="get" path="/accounting/offers/{offerId}" -->
```typescript
import { Maesn } from "maesn";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
});

async function run() {
  const result = await maesn.accounting.fetchOffer({
    offerId: "<id>",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { MaesnCore } from "maesn/core.js";
import { accountingFetchOffer } from "maesn/funcs/accounting-fetch-offer.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
});

async function run() {
  const res = await accountingFetchOffer(maesn, {
    offerId: "<id>",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("accountingFetchOffer failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.GetOfferRequest](../../models/operations/get-offer-request.md)                                                                                                     | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.GetOfferResponse](../../models/operations/get-offer-response.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |

## fetchOfferLineItems

### Example Usage

<!-- UsageSnippet language="typescript" operationID="getOfferLineItems" method="get" path="/accounting/offers/{offerId}/lineItems" -->
```typescript
import { Maesn } from "maesn";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
});

async function run() {
  const result = await maesn.accounting.fetchOfferLineItems({
    offerId: "<id>",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { MaesnCore } from "maesn/core.js";
import { accountingFetchOfferLineItems } from "maesn/funcs/accounting-fetch-offer-line-items.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
});

async function run() {
  const res = await accountingFetchOfferLineItems(maesn, {
    offerId: "<id>",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("accountingFetchOfferLineItems failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.GetOfferLineItemsRequest](../../models/operations/get-offer-line-items-request.md)                                                                                 | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.GetOfferLineItemsResponse](../../models/operations/get-offer-line-items-response.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |

## retrieveOfferLineItem

### Example Usage

<!-- UsageSnippet language="typescript" operationID="getOfferLineItem" method="get" path="/accounting/offers/{offerId}/lineItems/{lineItemId}" -->
```typescript
import { Maesn } from "maesn";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
});

async function run() {
  const result = await maesn.accounting.retrieveOfferLineItem({
    offerId: "<id>",
    lineItemId: "<id>",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { MaesnCore } from "maesn/core.js";
import { accountingRetrieveOfferLineItem } from "maesn/funcs/accounting-retrieve-offer-line-item.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
});

async function run() {
  const res = await accountingRetrieveOfferLineItem(maesn, {
    offerId: "<id>",
    lineItemId: "<id>",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("accountingRetrieveOfferLineItem failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.GetOfferLineItemRequest](../../models/operations/get-offer-line-item-request.md)                                                                                   | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.GetOfferLineItemResponse](../../models/operations/get-offer-line-item-response.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |

## addExpense

### Example Usage

<!-- UsageSnippet language="typescript" operationID="createExpense" method="post" path="/accounting/expenses" -->
```typescript
import { Maesn } from "maesn";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
});

async function run() {
  const result = await maesn.accounting.addExpense({
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
import { accountingAddExpense } from "maesn/funcs/accounting-add-expense.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
});

async function run() {
  const res = await accountingAddExpense(maesn, {
    body: {},
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("accountingAddExpense failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.CreateExpenseRequest](../../models/operations/create-expense-request.md)                                                                                           | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.CreateExpenseResponse](../../models/operations/create-expense-response.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |

## fetchExpenses

### Example Usage

<!-- UsageSnippet language="typescript" operationID="getExpenses" method="get" path="/accounting/expenses" -->
```typescript
import { Maesn } from "maesn";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
});

async function run() {
  const result = await maesn.accounting.fetchExpenses();

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { MaesnCore } from "maesn/core.js";
import { accountingFetchExpenses } from "maesn/funcs/accounting-fetch-expenses.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
});

async function run() {
  const res = await accountingFetchExpenses(maesn);
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("accountingFetchExpenses failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.GetExpensesRequest](../../models/operations/get-expenses-request.md)                                                                                               | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.GetExpensesResponse](../../models/operations/get-expenses-response.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |

## fetchExpense

### Example Usage

<!-- UsageSnippet language="typescript" operationID="getExpense" method="get" path="/accounting/expenses/{expenseId}" -->
```typescript
import { Maesn } from "maesn";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
});

async function run() {
  const result = await maesn.accounting.fetchExpense({
    expenseId: "<id>",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { MaesnCore } from "maesn/core.js";
import { accountingFetchExpense } from "maesn/funcs/accounting-fetch-expense.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
});

async function run() {
  const res = await accountingFetchExpense(maesn, {
    expenseId: "<id>",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("accountingFetchExpense failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.GetExpenseRequest](../../models/operations/get-expense-request.md)                                                                                                 | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.GetExpenseResponse](../../models/operations/get-expense-response.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |

## getProjects

### Example Usage

<!-- UsageSnippet language="typescript" operationID="getProjects" method="get" path="/accounting/projects" -->
```typescript
import { Maesn } from "maesn";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
});

async function run() {
  const result = await maesn.accounting.getProjects();

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { MaesnCore } from "maesn/core.js";
import { accountingGetProjects } from "maesn/funcs/accounting-get-projects.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
});

async function run() {
  const res = await accountingGetProjects(maesn);
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("accountingGetProjects failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.GetProjectsRequest](../../models/operations/get-projects-request.md)                                                                                               | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.GetProjectsResponse](../../models/operations/get-projects-response.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |

## addProject

### Example Usage

<!-- UsageSnippet language="typescript" operationID="createProject" method="post" path="/accounting/projects" -->
```typescript
import { Maesn } from "maesn";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
});

async function run() {
  const result = await maesn.accounting.addProject({
    body: {
      code: "<value>",
      contactId: "<id>",
      currency: "USD",
      description: "accidentally per justly inconsequential amidst",
      endDate: "<value>",
      name: "<value>",
      number: "<value>",
      parentProjectId: "<id>",
      status: "CLOSED",
      startDate: "<value>",
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
import { accountingAddProject } from "maesn/funcs/accounting-add-project.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
});

async function run() {
  const res = await accountingAddProject(maesn, {
    body: {
      code: "<value>",
      contactId: "<id>",
      currency: "USD",
      description: "accidentally per justly inconsequential amidst",
      endDate: "<value>",
      name: "<value>",
      number: "<value>",
      parentProjectId: "<id>",
      status: "CLOSED",
      startDate: "<value>",
    },
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("accountingAddProject failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.CreateProjectRequest](../../models/operations/create-project-request.md)                                                                                           | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.CreateProjectResponse](../../models/operations/create-project-response.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |

## fetchProject

### Example Usage

<!-- UsageSnippet language="typescript" operationID="getProject" method="get" path="/accounting/projects/{projectId}" -->
```typescript
import { Maesn } from "maesn";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
});

async function run() {
  const result = await maesn.accounting.fetchProject({
    projectId: "<id>",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { MaesnCore } from "maesn/core.js";
import { accountingFetchProject } from "maesn/funcs/accounting-fetch-project.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
});

async function run() {
  const res = await accountingFetchProject(maesn, {
    projectId: "<id>",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("accountingFetchProject failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.GetProjectRequest](../../models/operations/get-project-request.md)                                                                                                 | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.GetProjectResponse](../../models/operations/get-project-response.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |

## listSalesOrders

### Example Usage

<!-- UsageSnippet language="typescript" operationID="getSalesOrders" method="get" path="/accounting/salesOrders" -->
```typescript
import { Maesn } from "maesn";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
});

async function run() {
  const result = await maesn.accounting.listSalesOrders();

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { MaesnCore } from "maesn/core.js";
import { accountingListSalesOrders } from "maesn/funcs/accounting-list-sales-orders.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
});

async function run() {
  const res = await accountingListSalesOrders(maesn);
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("accountingListSalesOrders failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.GetSalesOrdersRequest](../../models/operations/get-sales-orders-request.md)                                                                                        | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.GetSalesOrdersResponse](../../models/operations/get-sales-orders-response.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |

## addSalesOrder

### Example Usage

<!-- UsageSnippet language="typescript" operationID="createSalesOrder" method="post" path="/accounting/salesOrders" -->
```typescript
import { Maesn } from "maesn";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
});

async function run() {
  const result = await maesn.accounting.addSalesOrder({
    body: {
      addresses: [
        {
          addressLine1: "896 Gulgowski Pass",
          addressLine2: "-",
          city: "Dickinsonland",
          countryCode: "TF",
          postalCode: "52370",
          type: "BILLING",
        },
      ],
      billingContactId: "<id>",
      comment: "The automobile layout consists of a front-engine design, with transaxle-type transmissions mounted at the rear of the engine and four wheel drive",
      contactId: "<id>",
      currency: "Rupiah",
      deliveryDate: "<value>",
      lineItems: [
        {
          itemId: "<id>",
          description: "immediately daughter moisten the yet",
          itemName: "<value>",
          quantity: 6426.16,
          taxCode: "<value>",
          taxRatePercentage: 6708.7,
          totalDiscountAmount: 7744.21,
          totalDiscountPercentage: 8362.05,
          totalGrossAmount: 2987.52,
          totalNetAmount: 7986.89,
          totalTaxAmount: 9981.01,
          unitAmount: 227.06,
          unitDiscountAmount: 3093.05,
          unitDiscountPercentage: 5819.56,
          unitName: "<value>",
        },
      ],
      oneLineAddress: "<value>",
      orderDate: "<value>",
      projectId: "<id>",
      shippingContactId: "<id>",
      status: "DRAFT",
      totalDiscountAmount: 8969.02,
      totalDiscountPercentage: 9154.02,
      totalGrossAmount: 5898.81,
      totalNetAmount: 3350.26,
      totalTaxAmount: 9404.22,
      version: "<value>",
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
import { accountingAddSalesOrder } from "maesn/funcs/accounting-add-sales-order.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
});

async function run() {
  const res = await accountingAddSalesOrder(maesn, {
    body: {
      addresses: [
        {
          addressLine1: "896 Gulgowski Pass",
          addressLine2: "-",
          city: "Dickinsonland",
          countryCode: "TF",
          postalCode: "52370",
          type: "BILLING",
        },
      ],
      billingContactId: "<id>",
      comment: "The automobile layout consists of a front-engine design, with transaxle-type transmissions mounted at the rear of the engine and four wheel drive",
      contactId: "<id>",
      currency: "Rupiah",
      deliveryDate: "<value>",
      lineItems: [
        {
          itemId: "<id>",
          description: "immediately daughter moisten the yet",
          itemName: "<value>",
          quantity: 6426.16,
          taxCode: "<value>",
          taxRatePercentage: 6708.7,
          totalDiscountAmount: 7744.21,
          totalDiscountPercentage: 8362.05,
          totalGrossAmount: 2987.52,
          totalNetAmount: 7986.89,
          totalTaxAmount: 9981.01,
          unitAmount: 227.06,
          unitDiscountAmount: 3093.05,
          unitDiscountPercentage: 5819.56,
          unitName: "<value>",
        },
      ],
      oneLineAddress: "<value>",
      orderDate: "<value>",
      projectId: "<id>",
      shippingContactId: "<id>",
      status: "DRAFT",
      totalDiscountAmount: 8969.02,
      totalDiscountPercentage: 9154.02,
      totalGrossAmount: 5898.81,
      totalNetAmount: 3350.26,
      totalTaxAmount: 9404.22,
      version: "<value>",
    },
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("accountingAddSalesOrder failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.CreateSalesOrderRequest](../../models/operations/create-sales-order-request.md)                                                                                    | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.CreateSalesOrderResponse](../../models/operations/create-sales-order-response.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |

## fetchSalesOrder

### Example Usage

<!-- UsageSnippet language="typescript" operationID="getSalesOrder" method="get" path="/accounting/salesOrders/{salesOrderId}" -->
```typescript
import { Maesn } from "maesn";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
});

async function run() {
  const result = await maesn.accounting.fetchSalesOrder({
    salesOrderId: "<id>",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { MaesnCore } from "maesn/core.js";
import { accountingFetchSalesOrder } from "maesn/funcs/accounting-fetch-sales-order.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
});

async function run() {
  const res = await accountingFetchSalesOrder(maesn, {
    salesOrderId: "<id>",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("accountingFetchSalesOrder failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.GetSalesOrderRequest](../../models/operations/get-sales-order-request.md)                                                                                          | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.GetSalesOrderResponse](../../models/operations/get-sales-order-response.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |

## listSalesOrderLineItems

### Example Usage

<!-- UsageSnippet language="typescript" operationID="getSalesOrderLines" method="get" path="/accounting/salesOrders/{salesOrderId}/lineItems" -->
```typescript
import { Maesn } from "maesn";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
});

async function run() {
  const result = await maesn.accounting.listSalesOrderLineItems({
    salesOrderId: "<id>",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { MaesnCore } from "maesn/core.js";
import { accountingListSalesOrderLineItems } from "maesn/funcs/accounting-list-sales-order-line-items.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
});

async function run() {
  const res = await accountingListSalesOrderLineItems(maesn, {
    salesOrderId: "<id>",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("accountingListSalesOrderLineItems failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.GetSalesOrderLinesRequest](../../models/operations/get-sales-order-lines-request.md)                                                                               | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.GetSalesOrderLinesResponse](../../models/operations/get-sales-order-lines-response.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |

## getPaymentTerms

### Example Usage

<!-- UsageSnippet language="typescript" operationID="getPaymentTerms" method="get" path="/accounting/paymentTerms" -->
```typescript
import { Maesn } from "maesn";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
});

async function run() {
  const result = await maesn.accounting.getPaymentTerms();

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { MaesnCore } from "maesn/core.js";
import { accountingGetPaymentTerms } from "maesn/funcs/accounting-get-payment-terms.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
});

async function run() {
  const res = await accountingGetPaymentTerms(maesn);
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("accountingGetPaymentTerms failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.GetPaymentTermsRequest](../../models/operations/get-payment-terms-request.md)                                                                                      | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.GetPaymentTermsResponse](../../models/operations/get-payment-terms-response.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |

## addPaymentTerm

### Example Usage

<!-- UsageSnippet language="typescript" operationID="createPaymentTerm" method="post" path="/accounting/paymentTerms" -->
```typescript
import { Maesn } from "maesn";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
});

async function run() {
  const result = await maesn.accounting.addPaymentTerm({
    body: {
      code: "<value>",
      description: "per forenenst quizzically justly hard-to-find abnormally serialize",
      discountDays: 289.02,
      discountDays2: 2344.82,
      discountPercentage: 2532.28,
      discountPercentage2: 1425.74,
      discountPeriods: [],
      dueType: "DUE_IN_DAYS",
      name: "<value>",
      paymentDays: 7137.87,
      paymentMethod: "<value>",
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
import { accountingAddPaymentTerm } from "maesn/funcs/accounting-add-payment-term.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
});

async function run() {
  const res = await accountingAddPaymentTerm(maesn, {
    body: {
      code: "<value>",
      description: "per forenenst quizzically justly hard-to-find abnormally serialize",
      discountDays: 289.02,
      discountDays2: 2344.82,
      discountPercentage: 2532.28,
      discountPercentage2: 1425.74,
      discountPeriods: [],
      dueType: "DUE_IN_DAYS",
      name: "<value>",
      paymentDays: 7137.87,
      paymentMethod: "<value>",
    },
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("accountingAddPaymentTerm failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.CreatePaymentTermRequest](../../models/operations/create-payment-term-request.md)                                                                                  | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.CreatePaymentTermResponse](../../models/operations/create-payment-term-response.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |

## fetchPaymentTerm

### Example Usage

<!-- UsageSnippet language="typescript" operationID="getPaymentTerm" method="get" path="/accounting/paymentTerms/{paymentTermId}" -->
```typescript
import { Maesn } from "maesn";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
});

async function run() {
  const result = await maesn.accounting.fetchPaymentTerm({
    paymentTermId: "<id>",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { MaesnCore } from "maesn/core.js";
import { accountingFetchPaymentTerm } from "maesn/funcs/accounting-fetch-payment-term.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
});

async function run() {
  const res = await accountingFetchPaymentTerm(maesn, {
    paymentTermId: "<id>",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("accountingFetchPaymentTerm failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.GetPaymentTermRequest](../../models/operations/get-payment-term-request.md)                                                                                        | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.GetPaymentTermResponse](../../models/operations/get-payment-term-response.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |

## retrieveTaxRates

### Example Usage

<!-- UsageSnippet language="typescript" operationID="getTaxRates" method="get" path="/accounting/taxRates" -->
```typescript
import { Maesn } from "maesn";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
});

async function run() {
  const result = await maesn.accounting.retrieveTaxRates();

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { MaesnCore } from "maesn/core.js";
import { accountingRetrieveTaxRates } from "maesn/funcs/accounting-retrieve-tax-rates.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
});

async function run() {
  const res = await accountingRetrieveTaxRates(maesn);
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("accountingRetrieveTaxRates failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.GetTaxRatesRequest](../../models/operations/get-tax-rates-request.md)                                                                                              | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.GetTaxRatesResponse](../../models/operations/get-tax-rates-response.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |

## fetchTaxRate

### Example Usage

<!-- UsageSnippet language="typescript" operationID="getTaxRate" method="get" path="/accounting/taxRates/{taxRateId}" -->
```typescript
import { Maesn } from "maesn";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
});

async function run() {
  const result = await maesn.accounting.fetchTaxRate({
    taxRateId: "<id>",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { MaesnCore } from "maesn/core.js";
import { accountingFetchTaxRate } from "maesn/funcs/accounting-fetch-tax-rate.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
});

async function run() {
  const res = await accountingFetchTaxRate(maesn, {
    taxRateId: "<id>",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("accountingFetchTaxRate failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.GetTaxRateRequest](../../models/operations/get-tax-rate-request.md)                                                                                                | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.GetTaxRateResponse](../../models/operations/get-tax-rate-response.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |

## retrievePayments

### Example Usage

<!-- UsageSnippet language="typescript" operationID="getPayments" method="get" path="/accounting/payments" -->
```typescript
import { Maesn } from "maesn";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
});

async function run() {
  const result = await maesn.accounting.retrievePayments();

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { MaesnCore } from "maesn/core.js";
import { accountingRetrievePayments } from "maesn/funcs/accounting-retrieve-payments.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
});

async function run() {
  const res = await accountingRetrievePayments(maesn);
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("accountingRetrievePayments failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.GetPaymentsRequest](../../models/operations/get-payments-request.md)                                                                                               | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.GetPaymentsResponse](../../models/operations/get-payments-response.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |

## addPayment

### Example Usage

<!-- UsageSnippet language="typescript" operationID="createPayment" method="post" path="/accounting/payments" -->
```typescript
import { Maesn } from "maesn";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
});

async function run() {
  const result = await maesn.accounting.addPayment({
    body: {
      currency: "Uganda Shilling",
      documentType: "<value>",
      exchangeRate: 9600.74,
      journalCode: "<value>",
      paymentType: "<value>",
      paymentLines: [
        {
          accountId: "<id>",
          amount: 3453.57,
          contactName: "<value>",
          customerId: "<id>",
          description: "up justly psst like",
          invoiceId: "<id>",
          supplierId: "<id>",
          paymentDate: "<value>",
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
import { MaesnCore } from "maesn/core.js";
import { accountingAddPayment } from "maesn/funcs/accounting-add-payment.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
});

async function run() {
  const res = await accountingAddPayment(maesn, {
    body: {
      currency: "Uganda Shilling",
      documentType: "<value>",
      exchangeRate: 9600.74,
      journalCode: "<value>",
      paymentType: "<value>",
      paymentLines: [
        {
          accountId: "<id>",
          amount: 3453.57,
          contactName: "<value>",
          customerId: "<id>",
          description: "up justly psst like",
          invoiceId: "<id>",
          supplierId: "<id>",
          paymentDate: "<value>",
        },
      ],
    },
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("accountingAddPayment failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.CreatePaymentRequest](../../models/operations/create-payment-request.md)                                                                                           | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.CreatePaymentResponse](../../models/operations/create-payment-response.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |

## fetchPayment

### Example Usage

<!-- UsageSnippet language="typescript" operationID="getPayment" method="get" path="/accounting/payments/{paymentId}" -->
```typescript
import { Maesn } from "maesn";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
});

async function run() {
  const result = await maesn.accounting.fetchPayment({
    paymentId: "<id>",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { MaesnCore } from "maesn/core.js";
import { accountingFetchPayment } from "maesn/funcs/accounting-fetch-payment.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
});

async function run() {
  const res = await accountingFetchPayment(maesn, {
    paymentId: "<id>",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("accountingFetchPayment failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.GetPaymentRequest](../../models/operations/get-payment-request.md)                                                                                                 | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.GetPaymentResponse](../../models/operations/get-payment-response.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |

## removePayment

### Example Usage

<!-- UsageSnippet language="typescript" operationID="deletePayment" method="delete" path="/accounting/payments/{paymentId}" -->
```typescript
import { Maesn } from "maesn";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
});

async function run() {
  await maesn.accounting.removePayment({
    paymentId: "<id>",
  });


}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { MaesnCore } from "maesn/core.js";
import { accountingRemovePayment } from "maesn/funcs/accounting-remove-payment.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
});

async function run() {
  const res = await accountingRemovePayment(maesn, {
    paymentId: "<id>",
  });
  if (res.ok) {
    const { value: result } = res;
    
  } else {
    console.log("accountingRemovePayment failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.DeletePaymentRequest](../../models/operations/delete-payment-request.md)                                                                                           | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<void\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |

## addEventSubscription

### Example Usage

<!-- UsageSnippet language="typescript" operationID="createEventSubscriptions" method="post" path="/accounting/event-subscriptions" -->
```typescript
import { Maesn } from "maesn";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
});

async function run() {
  await maesn.accounting.addEventSubscription({
    body: {
      eventType: "<value>",
      callbackUrl: "https://dark-vibraphone.com",
    },
  });


}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { MaesnCore } from "maesn/core.js";
import { accountingAddEventSubscription } from "maesn/funcs/accounting-add-event-subscription.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
});

async function run() {
  const res = await accountingAddEventSubscription(maesn, {
    body: {
      eventType: "<value>",
      callbackUrl: "https://dark-vibraphone.com",
    },
  });
  if (res.ok) {
    const { value: result } = res;
    
  } else {
    console.log("accountingAddEventSubscription failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.CreateEventSubscriptionsRequest](../../models/operations/create-event-subscriptions-request.md)                                                                    | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<void\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |

## removeEventSubscription

### Example Usage

<!-- UsageSnippet language="typescript" operationID="deleteEventSubscriptions" method="delete" path="/accounting/event-subscriptions/{eventSubscriptionId}" -->
```typescript
import { Maesn } from "maesn";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
});

async function run() {
  await maesn.accounting.removeEventSubscription({
    eventSubscriptionId: "<id>",
  });


}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { MaesnCore } from "maesn/core.js";
import { accountingRemoveEventSubscription } from "maesn/funcs/accounting-remove-event-subscription.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
});

async function run() {
  const res = await accountingRemoveEventSubscription(maesn, {
    eventSubscriptionId: "<id>",
  });
  if (res.ok) {
    const { value: result } = res;
    
  } else {
    console.log("accountingRemoveEventSubscription failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.DeleteEventSubscriptionsRequest](../../models/operations/delete-event-subscriptions-request.md)                                                                    | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<void\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |

## getProfile

### Example Usage

<!-- UsageSnippet language="typescript" operationID="getProfile" method="get" path="/accounting/profile" -->
```typescript
import { Maesn } from "maesn";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
});

async function run() {
  await maesn.accounting.getProfile();


}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { MaesnCore } from "maesn/core.js";
import { accountingGetProfile } from "maesn/funcs/accounting-get-profile.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
});

async function run() {
  const res = await accountingGetProfile(maesn);
  if (res.ok) {
    const { value: result } = res;
    
  } else {
    console.log("accountingGetProfile failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.GetProfileRequest](../../models/operations/get-profile-request.md)                                                                                                 | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<void\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |

## createPassThrough

### Example Usage

<!-- UsageSnippet language="typescript" operationID="createPassThroughRequest" method="post" path="/accounting/passThrough" -->
```typescript
import { Maesn } from "maesn";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
});

async function run() {
  const result = await maesn.accounting.createPassThrough({
    body: {
      path: "/usr/bin",
      method: "DELETE",
      headers: {},
      body: {},
      query: {},
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
import { accountingCreatePassThrough } from "maesn/funcs/accounting-create-pass-through.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
});

async function run() {
  const res = await accountingCreatePassThrough(maesn, {
    body: {
      path: "/usr/bin",
      method: "DELETE",
      headers: {},
      body: {},
      query: {},
    },
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("accountingCreatePassThrough failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.CreatePassThroughRequestRequest](../../models/operations/create-pass-through-request-request.md)                                                                   | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.CreatePassThroughRequestResponse](../../models/operations/create-pass-through-request-response.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |

## fetchBills

### Example Usage

<!-- UsageSnippet language="typescript" operationID="getBills" method="get" path="/accounting/bills" -->
```typescript
import { Maesn } from "maesn";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
});

async function run() {
  const result = await maesn.accounting.fetchBills();

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { MaesnCore } from "maesn/core.js";
import { accountingFetchBills } from "maesn/funcs/accounting-fetch-bills.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
});

async function run() {
  const res = await accountingFetchBills(maesn);
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("accountingFetchBills failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.GetBillsRequest](../../models/operations/get-bills-request.md)                                                                                                     | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.GetBillsResponse](../../models/operations/get-bills-response.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |

## addBill

### Example Usage

<!-- UsageSnippet language="typescript" operationID="createBill" method="post" path="/accounting/bills" -->
```typescript
import { Maesn } from "maesn";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
});

async function run() {
  const result = await maesn.accounting.addBill({
    body: {
      accountId: "<id>",
      addresses: [],
      billDate: "<value>",
      billNumber: "<value>",
      contactId: "<id>",
      currency: "Swiss Franc",
      deliveryDate: "<value>",
      dueDate: "<value>",
      fileId: "<id>",
      journalCode: "<value>",
      lineItems: [],
      name: "<value>",
      oneLineAddress: "<value>",
      paidDate: {},
      paymentTermCode: "<value>",
      paymentStatus: "NO_OPEN_ITEM",
      paymentDays: 7154.82,
      reference: "<value>",
      shippingDate: {},
      shippingType: "SERVICE",
      status: "DOCUMENT_CREATED",
      taxRule: "NON_DOMESTIC_SERVICE",
      taxText: "<value>",
      totalDiscountAmount: 8874.81,
      totalDiscountPercentage: 9973.49,
      totalGrossAmount: 190.3,
      totalNetAmount: 8970.07,
      totalTaxAmount: 3778.44,
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
import { accountingAddBill } from "maesn/funcs/accounting-add-bill.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
});

async function run() {
  const res = await accountingAddBill(maesn, {
    body: {
      accountId: "<id>",
      addresses: [],
      billDate: "<value>",
      billNumber: "<value>",
      contactId: "<id>",
      currency: "Swiss Franc",
      deliveryDate: "<value>",
      dueDate: "<value>",
      fileId: "<id>",
      journalCode: "<value>",
      lineItems: [],
      name: "<value>",
      oneLineAddress: "<value>",
      paidDate: {},
      paymentTermCode: "<value>",
      paymentStatus: "NO_OPEN_ITEM",
      paymentDays: 7154.82,
      reference: "<value>",
      shippingDate: {},
      shippingType: "SERVICE",
      status: "DOCUMENT_CREATED",
      taxRule: "NON_DOMESTIC_SERVICE",
      taxText: "<value>",
      totalDiscountAmount: 8874.81,
      totalDiscountPercentage: 9973.49,
      totalGrossAmount: 190.3,
      totalNetAmount: 8970.07,
      totalTaxAmount: 3778.44,
    },
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("accountingAddBill failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.CreateBillRequest](../../models/operations/create-bill-request.md)                                                                                                 | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.CreateBillResponse](../../models/operations/create-bill-response.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |

## fetchBill

### Example Usage

<!-- UsageSnippet language="typescript" operationID="getBill" method="get" path="/accounting/bills/{billId}" -->
```typescript
import { Maesn } from "maesn";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
});

async function run() {
  const result = await maesn.accounting.fetchBill({
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
import { accountingFetchBill } from "maesn/funcs/accounting-fetch-bill.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
});

async function run() {
  const res = await accountingFetchBill(maesn, {
    billId: "<id>",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("accountingFetchBill failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.GetBillRequest](../../models/operations/get-bill-request.md)                                                                                                       | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.GetBillResponse](../../models/operations/get-bill-response.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |

## removeBill

### Example Usage

<!-- UsageSnippet language="typescript" operationID="deleteBill" method="delete" path="/accounting/bills/{billId}" -->
```typescript
import { Maesn } from "maesn";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
});

async function run() {
  await maesn.accounting.removeBill({
    billId: "<id>",
  });


}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { MaesnCore } from "maesn/core.js";
import { accountingRemoveBill } from "maesn/funcs/accounting-remove-bill.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
});

async function run() {
  const res = await accountingRemoveBill(maesn, {
    billId: "<id>",
  });
  if (res.ok) {
    const { value: result } = res;
    
  } else {
    console.log("accountingRemoveBill failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.DeleteBillRequest](../../models/operations/delete-bill-request.md)                                                                                                 | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<void\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |

## fetchBillDocument

### Example Usage

<!-- UsageSnippet language="typescript" operationID="getBillDocument" method="get" path="/accounting/bills/{billId}/document" -->
```typescript
import { Maesn } from "maesn";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
});

async function run() {
  const result = await maesn.accounting.fetchBillDocument({
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
import { accountingFetchBillDocument } from "maesn/funcs/accounting-fetch-bill-document.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
});

async function run() {
  const res = await accountingFetchBillDocument(maesn, {
    billId: "<id>",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("accountingFetchBillDocument failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.GetBillDocumentRequest](../../models/operations/get-bill-document-request.md)                                                                                      | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.GetBillDocumentResponse](../../models/operations/get-bill-document-response.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |

## createBookingProposal

### Example Usage

<!-- UsageSnippet language="typescript" operationID="createBookingProposal" method="post" path="/accounting/bookingProposals" -->
```typescript
import { Maesn } from "maesn";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
});

async function run() {
  const result = await maesn.accounting.createBookingProposal({
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
import { accountingCreateBookingProposal } from "maesn/funcs/accounting-create-booking-proposal.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
});

async function run() {
  const res = await accountingCreateBookingProposal(maesn, {
    body: {},
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("accountingCreateBookingProposal failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.CreateBookingProposalRequest](../../models/operations/create-booking-proposal-request.md)                                                                          | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.CreateBookingProposalResponse](../../models/operations/create-booking-proposal-response.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |

## listBookingProposals

### Example Usage

<!-- UsageSnippet language="typescript" operationID="getBookingProposals" method="get" path="/accounting/bookingProposals" -->
```typescript
import { Maesn } from "maesn";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
});

async function run() {
  const result = await maesn.accounting.listBookingProposals();

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { MaesnCore } from "maesn/core.js";
import { accountingListBookingProposals } from "maesn/funcs/accounting-list-booking-proposals.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
});

async function run() {
  const res = await accountingListBookingProposals(maesn);
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("accountingListBookingProposals failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.GetBookingProposalsRequest](../../models/operations/get-booking-proposals-request.md)                                                                              | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.GetBookingProposalsResponse](../../models/operations/get-booking-proposals-response.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |

## retrieveBookingProposal

### Example Usage

<!-- UsageSnippet language="typescript" operationID="getBookingProposal" method="get" path="/accounting/bookingProposals/{bookingProposalId}" -->
```typescript
import { Maesn } from "maesn";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
});

async function run() {
  const result = await maesn.accounting.retrieveBookingProposal({
    bookingProposalId: "<id>",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { MaesnCore } from "maesn/core.js";
import { accountingRetrieveBookingProposal } from "maesn/funcs/accounting-retrieve-booking-proposal.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
});

async function run() {
  const res = await accountingRetrieveBookingProposal(maesn, {
    bookingProposalId: "<id>",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("accountingRetrieveBookingProposal failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.GetBookingProposalRequest](../../models/operations/get-booking-proposal-request.md)                                                                                | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.GetBookingProposalResponse](../../models/operations/get-booking-proposal-response.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |

## fetchBookingProposalDocument

### Example Usage

<!-- UsageSnippet language="typescript" operationID="getBookingProposalDocument" method="get" path="/accounting/bookingProposals/{bookingProposalId}/document" -->
```typescript
import { Maesn } from "maesn";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
});

async function run() {
  const result = await maesn.accounting.fetchBookingProposalDocument({
    bookingProposalId: "<id>",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { MaesnCore } from "maesn/core.js";
import { accountingFetchBookingProposalDocument } from "maesn/funcs/accounting-fetch-booking-proposal-document.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
});

async function run() {
  const res = await accountingFetchBookingProposalDocument(maesn, {
    bookingProposalId: "<id>",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("accountingFetchBookingProposalDocument failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.GetBookingProposalDocumentRequest](../../models/operations/get-booking-proposal-document-request.md)                                                               | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.GetBookingProposalDocumentResponse](../../models/operations/get-booking-proposal-document-response.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |

## addBooking

### Example Usage

<!-- UsageSnippet language="typescript" operationID="createBookings" method="post" path="/accounting/bookings" -->
```typescript
import { Maesn } from "maesn";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
});

async function run() {
  const result = await maesn.accounting.addBooking({
    body: {
      accountNumberLength: 6411.73,
      chartOfAccount: "SKR04",
      entries: [],
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
import { accountingAddBooking } from "maesn/funcs/accounting-add-booking.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
});

async function run() {
  const res = await accountingAddBooking(maesn, {
    body: {
      accountNumberLength: 6411.73,
      chartOfAccount: "SKR04",
      entries: [],
      fiscalYearStartDate: "<value>",
    },
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("accountingAddBooking failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.CreateBookingsRequest](../../models/operations/create-bookings-request.md)                                                                                         | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.CreateBookingsResponse](../../models/operations/create-bookings-response.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |

## retrieveVendorCredits

### Example Usage

<!-- UsageSnippet language="typescript" operationID="getVendorCredits" method="get" path="/accounting/vendorCredits" -->
```typescript
import { Maesn } from "maesn";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
});

async function run() {
  const result = await maesn.accounting.retrieveVendorCredits();

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { MaesnCore } from "maesn/core.js";
import { accountingRetrieveVendorCredits } from "maesn/funcs/accounting-retrieve-vendor-credits.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
});

async function run() {
  const res = await accountingRetrieveVendorCredits(maesn);
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("accountingRetrieveVendorCredits failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.GetVendorCreditsRequest](../../models/operations/get-vendor-credits-request.md)                                                                                    | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.GetVendorCreditsResponse](../../models/operations/get-vendor-credits-response.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |

## createVendorCredit

### Example Usage

<!-- UsageSnippet language="typescript" operationID="createVendorCredit" method="post" path="/accounting/vendorCredit" -->
```typescript
import { Maesn } from "maesn";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
});

async function run() {
  const result = await maesn.accounting.createVendorCredit({
    body: {
      accountId: "<id>",
      addresses: [
        {
          addressLine1: "861 Beech Drive",
          addressLine2: "-",
          city: "Palm Bay",
          countryCode: "GA",
          postalCode: "97113-7357",
          type: "BILLING",
        },
      ],
      contactId: "<id>",
      currency: "Zambian Kwacha",
      deliveryDate: "<value>",
      dueDate: "<value>",
      journalCode: "<value>",
      lineItems: [
        {
          id: "<id>",
          accountId: "<id>",
          accountNumber: "<value>",
          deferredEndDate: "<value>",
          deferredStartDate: "<value>",
          description: "parade behind whoa incidentally gloss what sate colorless mousse",
          dimensions: [],
          itemId: "<id>",
          itemName: "<value>",
          quantity: 2621.61,
          taxCode: "<value>",
          taxRatePercentage: 9944.31,
          totalDiscountAmount: 7042.22,
          totalDiscountPercentage: 791.91,
          totalGrossAmount: 3497.47,
          totalNetAmount: 982.03,
          totalTaxAmount: 4647.65,
          unitAmount: 763.74,
          unitDiscountAmount: 4173.63,
          unitDiscountPercentage: 9022.93,
          unitName: "<value>",
        },
      ],
      name: "<value>",
      oneLineAddress: "<value>",
      paidDate: {},
      paymentStatus: "PENDING",
      paymentDays: 5965.09,
      reference: "<value>",
      shippingDate: {},
      shippingType: "DELIVERY_PERIOD",
      status: "PARTIALLY_OVERDUE",
      taxRule: "NON_DOMESTIC_SERVICE",
      taxText: "<value>",
      totalDiscountAmount: 6759.1,
      totalDiscountPercentage: 8666.57,
      totalGrossAmount: 7760.69,
      totalNetAmount: 276.19,
      totalTaxAmount: 3591,
      vendorCreditDate: "<value>",
      vendorCreditNumber: "<value>",
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
import { accountingCreateVendorCredit } from "maesn/funcs/accounting-create-vendor-credit.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
});

async function run() {
  const res = await accountingCreateVendorCredit(maesn, {
    body: {
      accountId: "<id>",
      addresses: [
        {
          addressLine1: "861 Beech Drive",
          addressLine2: "-",
          city: "Palm Bay",
          countryCode: "GA",
          postalCode: "97113-7357",
          type: "BILLING",
        },
      ],
      contactId: "<id>",
      currency: "Zambian Kwacha",
      deliveryDate: "<value>",
      dueDate: "<value>",
      journalCode: "<value>",
      lineItems: [
        {
          id: "<id>",
          accountId: "<id>",
          accountNumber: "<value>",
          deferredEndDate: "<value>",
          deferredStartDate: "<value>",
          description: "parade behind whoa incidentally gloss what sate colorless mousse",
          dimensions: [],
          itemId: "<id>",
          itemName: "<value>",
          quantity: 2621.61,
          taxCode: "<value>",
          taxRatePercentage: 9944.31,
          totalDiscountAmount: 7042.22,
          totalDiscountPercentage: 791.91,
          totalGrossAmount: 3497.47,
          totalNetAmount: 982.03,
          totalTaxAmount: 4647.65,
          unitAmount: 763.74,
          unitDiscountAmount: 4173.63,
          unitDiscountPercentage: 9022.93,
          unitName: "<value>",
        },
      ],
      name: "<value>",
      oneLineAddress: "<value>",
      paidDate: {},
      paymentStatus: "PENDING",
      paymentDays: 5965.09,
      reference: "<value>",
      shippingDate: {},
      shippingType: "DELIVERY_PERIOD",
      status: "PARTIALLY_OVERDUE",
      taxRule: "NON_DOMESTIC_SERVICE",
      taxText: "<value>",
      totalDiscountAmount: 6759.1,
      totalDiscountPercentage: 8666.57,
      totalGrossAmount: 7760.69,
      totalNetAmount: 276.19,
      totalTaxAmount: 3591,
      vendorCreditDate: "<value>",
      vendorCreditNumber: "<value>",
    },
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("accountingCreateVendorCredit failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.CreateVendorCreditRequest](../../models/operations/create-vendor-credit-request.md)                                                                                | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.CreateVendorCreditResponse](../../models/operations/create-vendor-credit-response.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |

## modifyVendorCredit

### Example Usage

<!-- UsageSnippet language="typescript" operationID="updateVendorCredit" method="put" path="/accounting/vendorCredits/{vendorCreditId}" -->
```typescript
import { Maesn } from "maesn";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
});

async function run() {
  const result = await maesn.accounting.modifyVendorCredit({
    vendorCreditId: "<id>",
    body: {
      accountId: "<id>",
      addresses: [
        {
          addressLine1: "2914 Lancaster Road",
          addressLine2: "-",
          city: "Walkerborough",
          countryCode: "CG",
          postalCode: "17143",
          type: "BILLING",
        },
      ],
      contactId: "<id>",
      currency: "Kip",
      deliveryDate: "<value>",
      dueDate: "<value>",
      journalCode: "<value>",
      lineItems: [],
      name: "<value>",
      oneLineAddress: "<value>",
      paidDate: {},
      paymentStatus: "PARTIAL_CANCELLATION",
      paymentDays: 8588.89,
      reference: "<value>",
      shippingDate: {},
      shippingType: "DELIVERY_PERIOD",
      status: "OPEN",
      taxRule: "EXPORT_SERVICE",
      taxText: "<value>",
      totalDiscountAmount: 8650.66,
      totalDiscountPercentage: 9917.11,
      totalGrossAmount: 8449.02,
      totalNetAmount: 1897.58,
      totalTaxAmount: 7505.06,
      vendorCreditDate: "<value>",
      vendorCreditNumber: "<value>",
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
import { accountingModifyVendorCredit } from "maesn/funcs/accounting-modify-vendor-credit.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
});

async function run() {
  const res = await accountingModifyVendorCredit(maesn, {
    vendorCreditId: "<id>",
    body: {
      accountId: "<id>",
      addresses: [
        {
          addressLine1: "2914 Lancaster Road",
          addressLine2: "-",
          city: "Walkerborough",
          countryCode: "CG",
          postalCode: "17143",
          type: "BILLING",
        },
      ],
      contactId: "<id>",
      currency: "Kip",
      deliveryDate: "<value>",
      dueDate: "<value>",
      journalCode: "<value>",
      lineItems: [],
      name: "<value>",
      oneLineAddress: "<value>",
      paidDate: {},
      paymentStatus: "PARTIAL_CANCELLATION",
      paymentDays: 8588.89,
      reference: "<value>",
      shippingDate: {},
      shippingType: "DELIVERY_PERIOD",
      status: "OPEN",
      taxRule: "EXPORT_SERVICE",
      taxText: "<value>",
      totalDiscountAmount: 8650.66,
      totalDiscountPercentage: 9917.11,
      totalGrossAmount: 8449.02,
      totalNetAmount: 1897.58,
      totalTaxAmount: 7505.06,
      vendorCreditDate: "<value>",
      vendorCreditNumber: "<value>",
    },
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("accountingModifyVendorCredit failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.UpdateVendorCreditRequest](../../models/operations/update-vendor-credit-request.md)                                                                                | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.UpdateVendorCreditResponse](../../models/operations/update-vendor-credit-response.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |

## modifyBillLineItem

### Example Usage

<!-- UsageSnippet language="typescript" operationID="updateBillLineItem" method="put" path="/accounting/bills/{billId}/lineItems/{lineItemId}" -->
```typescript
import { Maesn } from "maesn";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
});

async function run() {
  const result = await maesn.accounting.modifyBillLineItem({
    billId: "<id>",
    lineItemId: "<id>",
    body: {
      id: "<id>",
      accountId: "<id>",
      accountNumber: "<value>",
      deferredEndDate: "<value>",
      deferredStartDate: "<value>",
      description: "bandwidth astride hm impolite discontinue surprisingly navigate",
      dimensions: [
        {
          name: "<value>",
          categoryName: "<value>",
        },
      ],
      itemId: "<id>",
      itemName: "<value>",
      quantity: 6276.63,
      taxCode: "<value>",
      taxRatePercentage: 9419.78,
      totalDiscountAmount: 9294.19,
      totalDiscountPercentage: 5782.96,
      totalGrossAmount: 4978.69,
      totalNetAmount: 9197.8,
      totalTaxAmount: 409.45,
      unitAmount: 8209.32,
      unitDiscountAmount: 3427.31,
      unitDiscountPercentage: 3142.63,
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
import { accountingModifyBillLineItem } from "maesn/funcs/accounting-modify-bill-line-item.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
});

async function run() {
  const res = await accountingModifyBillLineItem(maesn, {
    billId: "<id>",
    lineItemId: "<id>",
    body: {
      id: "<id>",
      accountId: "<id>",
      accountNumber: "<value>",
      deferredEndDate: "<value>",
      deferredStartDate: "<value>",
      description: "bandwidth astride hm impolite discontinue surprisingly navigate",
      dimensions: [
        {
          name: "<value>",
          categoryName: "<value>",
        },
      ],
      itemId: "<id>",
      itemName: "<value>",
      quantity: 6276.63,
      taxCode: "<value>",
      taxRatePercentage: 9419.78,
      totalDiscountAmount: 9294.19,
      totalDiscountPercentage: 5782.96,
      totalGrossAmount: 4978.69,
      totalNetAmount: 9197.8,
      totalTaxAmount: 409.45,
      unitAmount: 8209.32,
      unitDiscountAmount: 3427.31,
      unitDiscountPercentage: 3142.63,
      unitName: "<value>",
    },
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("accountingModifyBillLineItem failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.UpdateBillLineItemRequest](../../models/operations/update-bill-line-item-request.md)                                                                               | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.UpdateBillLineItemResponse](../../models/operations/update-bill-line-item-response.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |

## fetchPurchaseOrder

### Example Usage

<!-- UsageSnippet language="typescript" operationID="getPurchaseOrder" method="get" path="/accounting/purchaseOrders/{purchaseOrderId}" -->
```typescript
import { Maesn } from "maesn";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
});

async function run() {
  const result = await maesn.accounting.fetchPurchaseOrder({
    purchaseOrderId: "<id>",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { MaesnCore } from "maesn/core.js";
import { accountingFetchPurchaseOrder } from "maesn/funcs/accounting-fetch-purchase-order.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
});

async function run() {
  const res = await accountingFetchPurchaseOrder(maesn, {
    purchaseOrderId: "<id>",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("accountingFetchPurchaseOrder failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.GetPurchaseOrderRequest](../../models/operations/get-purchase-order-request.md)                                                                                    | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.GetPurchaseOrderResponse](../../models/operations/get-purchase-order-response.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |

## retrievePurchaseOrderLineItems

### Example Usage

<!-- UsageSnippet language="typescript" operationID="getPurchaseOrderLineItems" method="get" path="/accounting/purchaseOrders/{purchaseOrderId}/lineItems" -->
```typescript
import { Maesn } from "maesn";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
});

async function run() {
  const result = await maesn.accounting.retrievePurchaseOrderLineItems({
    purchaseOrderId: "<id>",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { MaesnCore } from "maesn/core.js";
import { accountingRetrievePurchaseOrderLineItems } from "maesn/funcs/accounting-retrieve-purchase-order-line-items.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
});

async function run() {
  const res = await accountingRetrievePurchaseOrderLineItems(maesn, {
    purchaseOrderId: "<id>",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("accountingRetrievePurchaseOrderLineItems failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.GetPurchaseOrderLineItemsRequest](../../models/operations/get-purchase-order-line-items-request.md)                                                                | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.GetPurchaseOrderLineItemsResponse](../../models/operations/get-purchase-order-line-items-response.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |

## retrievePurchaseOrderLineItem

### Example Usage

<!-- UsageSnippet language="typescript" operationID="getPurchaseOrderLineItem" method="get" path="/accounting/purchaseOrders/{purchaseOrderId}/lineItems/{lineItemId}" -->
```typescript
import { Maesn } from "maesn";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
});

async function run() {
  const result = await maesn.accounting.retrievePurchaseOrderLineItem({
    purchaseOrderId: "<id>",
    lineItemId: "<id>",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { MaesnCore } from "maesn/core.js";
import { accountingRetrievePurchaseOrderLineItem } from "maesn/funcs/accounting-retrieve-purchase-order-line-item.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
});

async function run() {
  const res = await accountingRetrievePurchaseOrderLineItem(maesn, {
    purchaseOrderId: "<id>",
    lineItemId: "<id>",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("accountingRetrievePurchaseOrderLineItem failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.GetPurchaseOrderLineItemRequest](../../models/operations/get-purchase-order-line-item-request.md)                                                                  | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.GetPurchaseOrderLineItemResponse](../../models/operations/get-purchase-order-line-item-response.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |

## getGoodsReceipts

### Example Usage

<!-- UsageSnippet language="typescript" operationID="getGoodsReceipts" method="get" path="/accounting/goodsReceipts" -->
```typescript
import { Maesn } from "maesn";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
});

async function run() {
  const result = await maesn.accounting.getGoodsReceipts();

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { MaesnCore } from "maesn/core.js";
import { accountingGetGoodsReceipts } from "maesn/funcs/accounting-get-goods-receipts.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
});

async function run() {
  const res = await accountingGetGoodsReceipts(maesn);
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("accountingGetGoodsReceipts failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.GetGoodsReceiptsRequest](../../models/operations/get-goods-receipts-request.md)                                                                                    | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.GetGoodsReceiptsResponse](../../models/operations/get-goods-receipts-response.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |

## retrieveGoodsReceipt

### Example Usage

<!-- UsageSnippet language="typescript" operationID="getGoodsReceipt" method="get" path="/accounting/goodsReceipts/{goodsReceiptId}" -->
```typescript
import { Maesn } from "maesn";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
});

async function run() {
  const result = await maesn.accounting.retrieveGoodsReceipt({
    goodsReceiptId: "<id>",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { MaesnCore } from "maesn/core.js";
import { accountingRetrieveGoodsReceipt } from "maesn/funcs/accounting-retrieve-goods-receipt.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
});

async function run() {
  const res = await accountingRetrieveGoodsReceipt(maesn, {
    goodsReceiptId: "<id>",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("accountingRetrieveGoodsReceipt failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.GetGoodsReceiptRequest](../../models/operations/get-goods-receipt-request.md)                                                                                      | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.GetGoodsReceiptResponse](../../models/operations/get-goods-receipt-response.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |

## retrieveGoodsReceiptLineItems

### Example Usage

<!-- UsageSnippet language="typescript" operationID="getGoodsReceiptLineItems" method="get" path="/accounting/goodsReceipts/{goodsReceiptId}/lineItems" -->
```typescript
import { Maesn } from "maesn";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
});

async function run() {
  const result = await maesn.accounting.retrieveGoodsReceiptLineItems({
    goodsReceiptId: "<id>",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { MaesnCore } from "maesn/core.js";
import { accountingRetrieveGoodsReceiptLineItems } from "maesn/funcs/accounting-retrieve-goods-receipt-line-items.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
});

async function run() {
  const res = await accountingRetrieveGoodsReceiptLineItems(maesn, {
    goodsReceiptId: "<id>",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("accountingRetrieveGoodsReceiptLineItems failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.GetGoodsReceiptLineItemsRequest](../../models/operations/get-goods-receipt-line-items-request.md)                                                                  | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.GetGoodsReceiptLineItemsResponse](../../models/operations/get-goods-receipt-line-items-response.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |

## fetchUnits

### Example Usage

<!-- UsageSnippet language="typescript" operationID="getUnits" method="get" path="/accounting/units" -->
```typescript
import { Maesn } from "maesn";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
});

async function run() {
  const result = await maesn.accounting.fetchUnits();

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { MaesnCore } from "maesn/core.js";
import { accountingFetchUnits } from "maesn/funcs/accounting-fetch-units.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
});

async function run() {
  const res = await accountingFetchUnits(maesn);
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("accountingFetchUnits failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.GetUnitsRequest](../../models/operations/get-units-request.md)                                                                                                     | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.GetUnitsResponse](../../models/operations/get-units-response.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |

## retrieveOpenItems

### Example Usage

<!-- UsageSnippet language="typescript" operationID="getOpenItems" method="get" path="/accounting/openItems" -->
```typescript
import { Maesn } from "maesn";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
});

async function run() {
  const result = await maesn.accounting.retrieveOpenItems();

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { MaesnCore } from "maesn/core.js";
import { accountingRetrieveOpenItems } from "maesn/funcs/accounting-retrieve-open-items.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
});

async function run() {
  const res = await accountingRetrieveOpenItems(maesn);
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("accountingRetrieveOpenItems failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.GetOpenItemsRequest](../../models/operations/get-open-items-request.md)                                                                                            | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.GetOpenItemsResponse](../../models/operations/get-open-items-response.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |

## fetchTrialBalance

### Example Usage

<!-- UsageSnippet language="typescript" operationID="getTrialBalance" method="get" path="/accounting/trialBalance" -->
```typescript
import { Maesn } from "maesn";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
});

async function run() {
  const result = await maesn.accounting.fetchTrialBalance();

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { MaesnCore } from "maesn/core.js";
import { accountingFetchTrialBalance } from "maesn/funcs/accounting-fetch-trial-balance.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
});

async function run() {
  const res = await accountingFetchTrialBalance(maesn);
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("accountingFetchTrialBalance failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.GetTrialBalanceRequest](../../models/operations/get-trial-balance-request.md)                                                                                      | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.GetTrialBalanceResponse](../../models/operations/get-trial-balance-response.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |

## listCreditNotes

### Example Usage

<!-- UsageSnippet language="typescript" operationID="getCreditNotes" method="get" path="/accounting/creditNotes" -->
```typescript
import { Maesn } from "maesn";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
});

async function run() {
  const result = await maesn.accounting.listCreditNotes();

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { MaesnCore } from "maesn/core.js";
import { accountingListCreditNotes } from "maesn/funcs/accounting-list-credit-notes.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
});

async function run() {
  const res = await accountingListCreditNotes(maesn);
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("accountingListCreditNotes failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.GetCreditNotesRequest](../../models/operations/get-credit-notes-request.md)                                                                                        | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.GetCreditNotesResponse](../../models/operations/get-credit-notes-response.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |

## fetchCreditNote

### Example Usage

<!-- UsageSnippet language="typescript" operationID="getCreditNote" method="get" path="/accounting/creditNotes/{creditNoteId}" -->
```typescript
import { Maesn } from "maesn";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
});

async function run() {
  const result = await maesn.accounting.fetchCreditNote({
    creditNoteId: "<id>",
  });

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { MaesnCore } from "maesn/core.js";
import { accountingFetchCreditNote } from "maesn/funcs/accounting-fetch-credit-note.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
});

async function run() {
  const res = await accountingFetchCreditNote(maesn, {
    creditNoteId: "<id>",
  });
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("accountingFetchCreditNote failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.GetCreditNoteRequest](../../models/operations/get-credit-note-request.md)                                                                                          | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.GetCreditNoteResponse](../../models/operations/get-credit-note-response.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |

## getFiscalYears

### Example Usage

<!-- UsageSnippet language="typescript" operationID="getFiscalYears" method="get" path="/accounting/fiscalYears" -->
```typescript
import { Maesn } from "maesn";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
});

async function run() {
  const result = await maesn.accounting.getFiscalYears();

  console.log(result);
}

run();
```

### Standalone function

The standalone function version of this method:

```typescript
import { MaesnCore } from "maesn/core.js";
import { accountingGetFiscalYears } from "maesn/funcs/accounting-get-fiscal-years.js";

// Use `MaesnCore` for best tree-shaking performance.
// You can create one instance of it to use across an application.
const maesn = new MaesnCore({
  serverURL: "https://api.example.com",
});

async function run() {
  const res = await accountingGetFiscalYears(maesn);
  if (res.ok) {
    const { value: result } = res;
    console.log(result);
  } else {
    console.log("accountingGetFiscalYears failed:", res.error);
  }
}

run();
```

### Parameters

| Parameter                                                                                                                                                                      | Type                                                                                                                                                                           | Required                                                                                                                                                                       | Description                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                                                                                      | [operations.GetFiscalYearsRequest](../../models/operations/get-fiscal-years-request.md)                                                                                        | :heavy_check_mark:                                                                                                                                                             | The request object to use for the request.                                                                                                                                     |
| `options`                                                                                                                                                                      | RequestOptions                                                                                                                                                                 | :heavy_minus_sign:                                                                                                                                                             | Used to set various options for making HTTP requests.                                                                                                                          |
| `options.fetchOptions`                                                                                                                                                         | [RequestInit](https://developer.mozilla.org/en-US/docs/Web/API/Request/Request#options)                                                                                        | :heavy_minus_sign:                                                                                                                                                             | Options that are passed to the underlying HTTP request. This can be used to inject extra headers for examples. All `Request` options, except `method` and `body`, are allowed. |
| `options.retries`                                                                                                                                                              | [RetryConfig](../../lib/utils/retryconfig.md)                                                                                                                                  | :heavy_minus_sign:                                                                                                                                                             | Enables retrying HTTP requests under certain failure conditions.                                                                                                               |

### Response

**Promise\<[operations.GetFiscalYearsResponse](../../models/operations/get-fiscal-years-response.md)\>**

### Errors

| Error Type               | Status Code              | Content Type             |
| ------------------------ | ------------------------ | ------------------------ |
| errors.MaesnDefaultError | 4XX, 5XX                 | \*/\*                    |