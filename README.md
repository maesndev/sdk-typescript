# maesn

Developer-friendly & type-safe Typescript SDK specifically catered to leverage *maesn* API.

[![Built by Speakeasy](https://img.shields.io/badge/Built_by-SPEAKEASY-374151?style=for-the-badge&labelColor=f3f4f6)](https://www.speakeasy.com/?utm_source=maesn&utm_campaign=typescript)
[![License: MIT](https://img.shields.io/badge/LICENSE_//_MIT-3b5bdb?style=for-the-badge&labelColor=eff6ff)](https://opensource.org/licenses/MIT)


<!-- Start Summary [summary] -->
## Summary

Maesn Unified API: The Maesn Unified API provides a single interface to 30+ accounting and ERP target systems — including Exact, Xero, Sevdesk, Lexoffice, QuickBooks, DATEV, FreshBooks, and more.

All resources (invoices, contacts, accounts, bills, journal entries, payments) are normalized to a common schema, so your integration works across every connected system without modification.

## Features

- **Unified schema** — one data model across all target systems
- **Multi-tenant** — isolated API keys and account keys per tenant and end user
- **OAuth integration** — built-in OAuth flows for all supported target systems
- **Webhook support** — subscribe to real-time events from connected target systems
- **Async processing** — long-running operations return a `taskId` for status polling
<!-- End Summary [summary] -->

<!-- Start Table of Contents [toc] -->
## Table of Contents
<!-- $toc-max-depth=2 -->
* [maesn](#maesn)
  * [Features](#features)
  * [SDK Installation](#sdk-installation)
  * [Requirements](#requirements)
  * [SDK Example Usage](#sdk-example-usage)
  * [Authentication](#authentication)
  * [Available Resources and Operations](#available-resources-and-operations)
  * [Standalone functions](#standalone-functions)
  * [File uploads](#file-uploads)
  * [Retries](#retries)
  * [Error Handling](#error-handling)
  * [Custom HTTP Client](#custom-http-client)
  * [Debugging](#debugging)
* [Development](#development)
  * [Maturity](#maturity)
  * [Contributions](#contributions)

<!-- End Table of Contents [toc] -->

<!-- Start SDK Installation [installation] -->
## SDK Installation

The SDK can be installed with either [npm](https://www.npmjs.com/), [pnpm](https://pnpm.io/), [bun](https://bun.sh/) or [yarn](https://classic.yarnpkg.com/en/) package managers.

### NPM

```bash
npm add @maesn/typescript-sdk
```

### PNPM

```bash
pnpm add @maesn/typescript-sdk
```

### Bun

```bash
bun add @maesn/typescript-sdk
```

### Yarn

```bash
yarn add @maesn/typescript-sdk
```

> [!NOTE]
> This package is published as an ES Module (ESM) only. For applications using
> CommonJS, use `await import("@maesn/typescript-sdk")` to import and use this package.
<!-- End SDK Installation [installation] -->

<!-- Start Requirements [requirements] -->
## Requirements

For supported JavaScript runtimes, please consult [RUNTIMES.md](RUNTIMES.md).
<!-- End Requirements [requirements] -->

<!-- Start SDK Example Usage [usage] -->
## SDK Example Usage

### Example

```typescript
import { Maesn } from "@maesn/typescript-sdk";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
  security: {
    apiKey: process.env["MAESN_API_KEY"] ?? "",
    accountKey: process.env["MAESN_ACCOUNT_KEY"] ?? "",
  },
});

async function run() {
  const result = await maesn.accounting.retrieveAccount({
    accountId: "<id>",
  });

  console.log(result);
}

run();

```
<!-- End SDK Example Usage [usage] -->

<!-- Start Authentication [security] -->
## Authentication

### Per-Client Security Schemes

This SDK supports the following security schemes globally:

| Name         | Type   | Scheme  | Environment Variable |
| ------------ | ------ | ------- | -------------------- |
| `apiKey`     | apiKey | API key | `MAESN_API_KEY`      |
| `accountKey` | apiKey | API key | `MAESN_ACCOUNT_KEY`  |

You can set the security parameters through the `security` optional parameter when initializing the SDK client instance. The selected scheme will be used by default to authenticate with the API for all operations that support it. For example:
```typescript
import { Maesn } from "@maesn/typescript-sdk";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
  security: {
    apiKey: process.env["MAESN_API_KEY"] ?? "",
    accountKey: process.env["MAESN_ACCOUNT_KEY"] ?? "",
  },
});

async function run() {
  const result = await maesn.accounting.retrieveAccount({
    accountId: "<id>",
  });

  console.log(result);
}

run();

```
<!-- End Authentication [security] -->

<!-- Start Available Resources and Operations [operations] -->
## Available Resources and Operations

<details open>
<summary>Available methods</summary>

### [Accounting](docs/sdks/accounting/README.md)

* [retrieveAccount](docs/sdks/accounting/README.md#retrieveaccount)
* [retrieveAccounts](docs/sdks/accounting/README.md#retrieveaccounts)
* [addAccount](docs/sdks/accounting/README.md#addaccount)
* [retrieveBankAccounts](docs/sdks/accounting/README.md#retrievebankaccounts)
* [addBankAccount](docs/sdks/accounting/README.md#addbankaccount)
* [fetchBankAccount](docs/sdks/accounting/README.md#fetchbankaccount)
* [retrieveDimensions](docs/sdks/accounting/README.md#retrievedimensions)
* [recordTransaction](docs/sdks/accounting/README.md#recordtransaction)
* [fetchCustomers](docs/sdks/accounting/README.md#fetchcustomers)
* [createCustomer](docs/sdks/accounting/README.md#createcustomer)
* [fetchCustomer](docs/sdks/accounting/README.md#fetchcustomer)
* [updateCustomer](docs/sdks/accounting/README.md#updatecustomer)
* [amendCustomer](docs/sdks/accounting/README.md#amendcustomer)
* [retrieveSuppliers](docs/sdks/accounting/README.md#retrievesuppliers)
* [addSupplier](docs/sdks/accounting/README.md#addsupplier)
* [fetchSupplier](docs/sdks/accounting/README.md#fetchsupplier)
* [modifySupplier](docs/sdks/accounting/README.md#modifysupplier)
* [amendSupplier](docs/sdks/accounting/README.md#amendsupplier)
* [getContacts](docs/sdks/accounting/README.md#getcontacts)
* [addContact](docs/sdks/accounting/README.md#addcontact)
* [fetchContact](docs/sdks/accounting/README.md#fetchcontact)
* [replaceContact](docs/sdks/accounting/README.md#replacecontact)
* [createContactsBulk](docs/sdks/accounting/README.md#createcontactsbulk)
* [batchAddContacts](docs/sdks/accounting/README.md#batchaddcontacts)
* [retrieveInvoices](docs/sdks/accounting/README.md#retrieveinvoices)
* [addInvoice](docs/sdks/accounting/README.md#addinvoice)
* [fetchInvoice](docs/sdks/accounting/README.md#fetchinvoice)
* [amendInvoice](docs/sdks/accounting/README.md#amendinvoice)
* [fetchInvoiceDocument](docs/sdks/accounting/README.md#fetchinvoicedocument)
* [uploadFile](docs/sdks/accounting/README.md#uploadfile)
* [fetchDocumentTypes](docs/sdks/accounting/README.md#fetchdocumenttypes)
* [getAsyncTask](docs/sdks/accounting/README.md#getasynctask)
* [retrieveItems](docs/sdks/accounting/README.md#retrieveitems)
* [fetchItem](docs/sdks/accounting/README.md#fetchitem)
* [retrieveInvoiceLineItems](docs/sdks/accounting/README.md#retrieveinvoicelineitems)
* [addInvoiceLineItem](docs/sdks/accounting/README.md#addinvoicelineitem)
* [retrieveInvoiceLineItem](docs/sdks/accounting/README.md#retrieveinvoicelineitem)
* [fetchJournals](docs/sdks/accounting/README.md#fetchjournals)
* [listJournalEntries](docs/sdks/accounting/README.md#listjournalentries)
* [addJournalEntry](docs/sdks/accounting/README.md#addjournalentry)
* [fetchJournalEntry](docs/sdks/accounting/README.md#fetchjournalentry)
* [createJournalEntryAttachments](docs/sdks/accounting/README.md#createjournalentryattachments)
* [fetchOffers](docs/sdks/accounting/README.md#fetchoffers)
* [addOffer](docs/sdks/accounting/README.md#addoffer)
* [fetchOffer](docs/sdks/accounting/README.md#fetchoffer)
* [fetchOfferLineItems](docs/sdks/accounting/README.md#fetchofferlineitems)
* [retrieveOfferLineItem](docs/sdks/accounting/README.md#retrieveofferlineitem)
* [addExpense](docs/sdks/accounting/README.md#addexpense)
* [fetchExpenses](docs/sdks/accounting/README.md#fetchexpenses)
* [fetchExpense](docs/sdks/accounting/README.md#fetchexpense)
* [getProjects](docs/sdks/accounting/README.md#getprojects)
* [addProject](docs/sdks/accounting/README.md#addproject)
* [fetchProject](docs/sdks/accounting/README.md#fetchproject)
* [listSalesOrders](docs/sdks/accounting/README.md#listsalesorders)
* [addSalesOrder](docs/sdks/accounting/README.md#addsalesorder)
* [fetchSalesOrder](docs/sdks/accounting/README.md#fetchsalesorder)
* [listSalesOrderLineItems](docs/sdks/accounting/README.md#listsalesorderlineitems)
* [getPaymentTerms](docs/sdks/accounting/README.md#getpaymentterms)
* [addPaymentTerm](docs/sdks/accounting/README.md#addpaymentterm)
* [fetchPaymentTerm](docs/sdks/accounting/README.md#fetchpaymentterm)
* [retrieveTaxRates](docs/sdks/accounting/README.md#retrievetaxrates)
* [fetchTaxRate](docs/sdks/accounting/README.md#fetchtaxrate)
* [retrievePayments](docs/sdks/accounting/README.md#retrievepayments)
* [addPayment](docs/sdks/accounting/README.md#addpayment)
* [fetchPayment](docs/sdks/accounting/README.md#fetchpayment)
* [removePayment](docs/sdks/accounting/README.md#removepayment)
* [addEventSubscription](docs/sdks/accounting/README.md#addeventsubscription)
* [removeEventSubscription](docs/sdks/accounting/README.md#removeeventsubscription)
* [getProfile](docs/sdks/accounting/README.md#getprofile)
* [createPassThrough](docs/sdks/accounting/README.md#createpassthrough)
* [fetchBills](docs/sdks/accounting/README.md#fetchbills)
* [addBill](docs/sdks/accounting/README.md#addbill)
* [fetchBill](docs/sdks/accounting/README.md#fetchbill)
* [removeBill](docs/sdks/accounting/README.md#removebill)
* [fetchBillDocument](docs/sdks/accounting/README.md#fetchbilldocument)
* [createBookingProposal](docs/sdks/accounting/README.md#createbookingproposal)
* [listBookingProposals](docs/sdks/accounting/README.md#listbookingproposals)
* [retrieveBookingProposal](docs/sdks/accounting/README.md#retrievebookingproposal)
* [fetchBookingProposalDocument](docs/sdks/accounting/README.md#fetchbookingproposaldocument)
* [addBooking](docs/sdks/accounting/README.md#addbooking)
* [retrieveVendorCredits](docs/sdks/accounting/README.md#retrievevendorcredits)
* [createVendorCredit](docs/sdks/accounting/README.md#createvendorcredit)
* [modifyVendorCredit](docs/sdks/accounting/README.md#modifyvendorcredit)
* [modifyBillLineItem](docs/sdks/accounting/README.md#modifybilllineitem)
* [fetchPurchaseOrder](docs/sdks/accounting/README.md#fetchpurchaseorder)
* [retrievePurchaseOrderLineItems](docs/sdks/accounting/README.md#retrievepurchaseorderlineitems)
* [retrievePurchaseOrderLineItem](docs/sdks/accounting/README.md#retrievepurchaseorderlineitem)
* [getGoodsReceipts](docs/sdks/accounting/README.md#getgoodsreceipts)
* [retrieveGoodsReceipt](docs/sdks/accounting/README.md#retrievegoodsreceipt)
* [retrieveGoodsReceiptLineItems](docs/sdks/accounting/README.md#retrievegoodsreceiptlineitems)
* [fetchUnits](docs/sdks/accounting/README.md#fetchunits)
* [retrieveOpenItems](docs/sdks/accounting/README.md#retrieveopenitems)
* [fetchTrialBalance](docs/sdks/accounting/README.md#fetchtrialbalance)
* [listCreditNotes](docs/sdks/accounting/README.md#listcreditnotes)
* [fetchCreditNote](docs/sdks/accounting/README.md#fetchcreditnote)
* [getFiscalYears](docs/sdks/accounting/README.md#getfiscalyears)

#### [Accounting.Bills](docs/sdks/accountingbills/README.md)

* [addLineItem](docs/sdks/accountingbills/README.md#addlineitem)

#### [Accounting.Invoices](docs/sdks/invoices/README.md)

* [updateLineItem](docs/sdks/invoices/README.md#updatelineitem)

#### [Accounting.JournalEntries](docs/sdks/accountingjournalentries/README.md)

* [getAttachments](docs/sdks/accountingjournalentries/README.md#getattachments)

#### [Accounting.V2](docs/sdks/v2/README.md)

* [getDimension](docs/sdks/v2/README.md#getdimension)

##### [Accounting.V2.Contacts](docs/sdks/v2contacts/README.md)

* [update](docs/sdks/v2contacts/README.md#update)

### [AccountingV2](docs/sdks/accountingv2/README.md)

* [createBookingProposal](docs/sdks/accountingv2/README.md#createbookingproposal)
* [createContact](docs/sdks/accountingv2/README.md#createcontact)
* [updateContact](docs/sdks/accountingv2/README.md#updatecontact)
* [obtainDimensions](docs/sdks/accountingv2/README.md#obtaindimensions)

### [Auth](docs/sdks/auth/README.md)

* [getEnvironments](docs/sdks/auth/README.md#getenvironments)
* [getCompanies](docs/sdks/auth/README.md#getcompanies)
* [getCompaniesFlow](docs/sdks/auth/README.md#getcompaniesflow)
* [getSubmitPage](docs/sdks/auth/README.md#getsubmitpage)
* [apiKeyConfirmation](docs/sdks/auth/README.md#apikeyconfirmation)
* [cancel](docs/sdks/auth/README.md#cancel)
* [test](docs/sdks/auth/README.md#test)
* [longToken](docs/sdks/auth/README.md#longtoken)
* [getEnvironmentPage](docs/sdks/auth/README.md#getenvironmentpage)
* [setEndUserSelections](docs/sdks/auth/README.md#setenduserselections)
* [systemLoginUrl](docs/sdks/auth/README.md#systemloginurl)
* [callback](docs/sdks/auth/README.md#callback)
* [createEndUserAccount](docs/sdks/auth/README.md#createenduseraccount)

### [Bills](docs/sdks/bills/README.md)

* [update](docs/sdks/bills/README.md#update)
* [getLineItems](docs/sdks/bills/README.md#getlineitems)

### [Contacts](docs/sdks/contacts/README.md)

* [patch](docs/sdks/contacts/README.md#patch)

### [ContactsV2](docs/sdks/contactsv2/README.md)

* [list](docs/sdks/contactsv2/README.md#list)
* [get](docs/sdks/contactsv2/README.md#get)

### [Events](docs/sdks/events/README.md)

* [handleCallback](docs/sdks/events/README.md#handlecallback)
* [getCode](docs/sdks/events/README.md#getcode)
* [handleConfigurationCallback](docs/sdks/events/README.md#handleconfigurationcallback)

### [Files](docs/sdks/files/README.md)

* [getDocumentExtensions](docs/sdks/files/README.md#getdocumentextensions)

### [FiscalYears](docs/sdks/fiscalyears/README.md)

* [get](docs/sdks/fiscalyears/README.md#get)

### [GoodsReceipts](docs/sdks/goodsreceipts/README.md)

* [getLineItem](docs/sdks/goodsreceipts/README.md#getlineitem)

### [Health](docs/sdks/health/README.md)

* [check](docs/sdks/health/README.md#check) - Health check
* [details](docs/sdks/health/README.md#details) - Detailed health check

### [Items](docs/sdks/items/README.md)

* [create](docs/sdks/items/README.md#create)
* [modify](docs/sdks/items/README.md#modify)

### [JournalEntries](docs/sdks/journalentries/README.md)

* [createBulk](docs/sdks/journalentries/README.md#createbulk)

### [JournalEntryAttachments](docs/sdks/journalentryattachments/README.md)

* [getById](docs/sdks/journalentryattachments/README.md#getbyid)

### [Offers](docs/sdks/offers/README.md)

* [getDocument](docs/sdks/offers/README.md#getdocument)

### [PurchaseOrders](docs/sdks/purchaseorders/README.md)

* [list](docs/sdks/purchaseorders/README.md#list)

### [Tenants](docs/sdks/tenants/README.md)

* [systemRegistration](docs/sdks/tenants/README.md#systemregistration)
* [addCallbackUrl](docs/sdks/tenants/README.md#addcallbackurl)
* [getEndUserList](docs/sdks/tenants/README.md#getenduserlist)
* [countEndUsersBySystem](docs/sdks/tenants/README.md#countendusersbysystem)
* [deleteEndUser](docs/sdks/tenants/README.md#deleteenduser)
* [getCallbackUrl](docs/sdks/tenants/README.md#getcallbackurl)
* [getRegisteredSystems](docs/sdks/tenants/README.md#getregisteredsystems)
* [getTargetSystemValues](docs/sdks/tenants/README.md#gettargetsystemvalues)
* [getTargetSystemRequirements](docs/sdks/tenants/README.md#gettargetsystemrequirements)
* [getRegisteredSystemsMasked](docs/sdks/tenants/README.md#getregisteredsystemsmasked)
* [deleteRegisteredSystem](docs/sdks/tenants/README.md#deleteregisteredsystem)
* [getAllActiveEndUsers](docs/sdks/tenants/README.md#getallactiveendusers)
* [getSubmissionPageStyle](docs/sdks/tenants/README.md#getsubmissionpagestyle)
* [updateSubmissionPageStyle](docs/sdks/tenants/README.md#updatesubmissionpagestyle)
* [getSubmissionPageStyleByKey](docs/sdks/tenants/README.md#getsubmissionpagestylebykey)

### [User](docs/sdks/user/README.md)

* [getInfo](docs/sdks/user/README.md#getinfo)

### [VendorCredits](docs/sdks/vendorcredits/README.md)

* [delete](docs/sdks/vendorcredits/README.md#delete)

### [Webhooks](docs/sdks/webhooks/README.md)

* [createWebhookEndUser](docs/sdks/webhooks/README.md#createwebhookenduser)
* [createWebHookTenant](docs/sdks/webhooks/README.md#createwebhooktenant)
* [deleteWebhookEndUser](docs/sdks/webhooks/README.md#deletewebhookenduser)
* [deleteWebhookTenant](docs/sdks/webhooks/README.md#deletewebhooktenant)
* [createWebhookConfig](docs/sdks/webhooks/README.md#createwebhookconfig)
* [createWebhook](docs/sdks/webhooks/README.md#createwebhook)
* [deleteWebhook](docs/sdks/webhooks/README.md#deletewebhook)
* [getWebhooks](docs/sdks/webhooks/README.md#getwebhooks)

</details>
<!-- End Available Resources and Operations [operations] -->

<!-- Start Standalone functions [standalone-funcs] -->
## Standalone functions

All the methods listed above are available as standalone functions. These
functions are ideal for use in applications running in the browser, serverless
runtimes or other environments where application bundle size is a primary
concern. When using a bundler to build your application, all unused
functionality will be either excluded from the final bundle or tree-shaken away.

To read more about standalone functions, check [FUNCTIONS.md](./FUNCTIONS.md).

<details>

<summary>Available standalone functions</summary>

- [`accountingAddAccount`](docs/sdks/accounting/README.md#addaccount)
- [`accountingAddBankAccount`](docs/sdks/accounting/README.md#addbankaccount)
- [`accountingAddBill`](docs/sdks/accounting/README.md#addbill)
- [`accountingAddBooking`](docs/sdks/accounting/README.md#addbooking)
- [`accountingAddContact`](docs/sdks/accounting/README.md#addcontact)
- [`accountingAddEventSubscription`](docs/sdks/accounting/README.md#addeventsubscription)
- [`accountingAddExpense`](docs/sdks/accounting/README.md#addexpense)
- [`accountingAddInvoice`](docs/sdks/accounting/README.md#addinvoice)
- [`accountingAddInvoiceLineItem`](docs/sdks/accounting/README.md#addinvoicelineitem)
- [`accountingAddJournalEntry`](docs/sdks/accounting/README.md#addjournalentry)
- [`accountingAddOffer`](docs/sdks/accounting/README.md#addoffer)
- [`accountingAddPayment`](docs/sdks/accounting/README.md#addpayment)
- [`accountingAddPaymentTerm`](docs/sdks/accounting/README.md#addpaymentterm)
- [`accountingAddProject`](docs/sdks/accounting/README.md#addproject)
- [`accountingAddSalesOrder`](docs/sdks/accounting/README.md#addsalesorder)
- [`accountingAddSupplier`](docs/sdks/accounting/README.md#addsupplier)
- [`accountingAmendCustomer`](docs/sdks/accounting/README.md#amendcustomer)
- [`accountingAmendInvoice`](docs/sdks/accounting/README.md#amendinvoice)
- [`accountingAmendSupplier`](docs/sdks/accounting/README.md#amendsupplier)
- [`accountingBatchAddContacts`](docs/sdks/accounting/README.md#batchaddcontacts)
- [`accountingBillsAddLineItem`](docs/sdks/accountingbills/README.md#addlineitem)
- [`accountingCreateBookingProposal`](docs/sdks/accounting/README.md#createbookingproposal)
- [`accountingCreateContactsBulk`](docs/sdks/accounting/README.md#createcontactsbulk)
- [`accountingCreateCustomer`](docs/sdks/accounting/README.md#createcustomer)
- [`accountingCreateJournalEntryAttachments`](docs/sdks/accounting/README.md#createjournalentryattachments)
- [`accountingCreatePassThrough`](docs/sdks/accounting/README.md#createpassthrough)
- [`accountingCreateVendorCredit`](docs/sdks/accounting/README.md#createvendorcredit)
- [`accountingFetchBankAccount`](docs/sdks/accounting/README.md#fetchbankaccount)
- [`accountingFetchBill`](docs/sdks/accounting/README.md#fetchbill)
- [`accountingFetchBillDocument`](docs/sdks/accounting/README.md#fetchbilldocument)
- [`accountingFetchBills`](docs/sdks/accounting/README.md#fetchbills)
- [`accountingFetchBookingProposalDocument`](docs/sdks/accounting/README.md#fetchbookingproposaldocument)
- [`accountingFetchContact`](docs/sdks/accounting/README.md#fetchcontact)
- [`accountingFetchCreditNote`](docs/sdks/accounting/README.md#fetchcreditnote)
- [`accountingFetchCustomer`](docs/sdks/accounting/README.md#fetchcustomer)
- [`accountingFetchCustomers`](docs/sdks/accounting/README.md#fetchcustomers)
- [`accountingFetchDocumentTypes`](docs/sdks/accounting/README.md#fetchdocumenttypes)
- [`accountingFetchExpense`](docs/sdks/accounting/README.md#fetchexpense)
- [`accountingFetchExpenses`](docs/sdks/accounting/README.md#fetchexpenses)
- [`accountingFetchInvoice`](docs/sdks/accounting/README.md#fetchinvoice)
- [`accountingFetchInvoiceDocument`](docs/sdks/accounting/README.md#fetchinvoicedocument)
- [`accountingFetchItem`](docs/sdks/accounting/README.md#fetchitem)
- [`accountingFetchJournalEntry`](docs/sdks/accounting/README.md#fetchjournalentry)
- [`accountingFetchJournals`](docs/sdks/accounting/README.md#fetchjournals)
- [`accountingFetchOffer`](docs/sdks/accounting/README.md#fetchoffer)
- [`accountingFetchOfferLineItems`](docs/sdks/accounting/README.md#fetchofferlineitems)
- [`accountingFetchOffers`](docs/sdks/accounting/README.md#fetchoffers)
- [`accountingFetchPayment`](docs/sdks/accounting/README.md#fetchpayment)
- [`accountingFetchPaymentTerm`](docs/sdks/accounting/README.md#fetchpaymentterm)
- [`accountingFetchProject`](docs/sdks/accounting/README.md#fetchproject)
- [`accountingFetchPurchaseOrder`](docs/sdks/accounting/README.md#fetchpurchaseorder)
- [`accountingFetchSalesOrder`](docs/sdks/accounting/README.md#fetchsalesorder)
- [`accountingFetchSupplier`](docs/sdks/accounting/README.md#fetchsupplier)
- [`accountingFetchTaxRate`](docs/sdks/accounting/README.md#fetchtaxrate)
- [`accountingFetchTrialBalance`](docs/sdks/accounting/README.md#fetchtrialbalance)
- [`accountingFetchUnits`](docs/sdks/accounting/README.md#fetchunits)
- [`accountingGetAsyncTask`](docs/sdks/accounting/README.md#getasynctask)
- [`accountingGetContacts`](docs/sdks/accounting/README.md#getcontacts)
- [`accountingGetFiscalYears`](docs/sdks/accounting/README.md#getfiscalyears)
- [`accountingGetGoodsReceipts`](docs/sdks/accounting/README.md#getgoodsreceipts)
- [`accountingGetPaymentTerms`](docs/sdks/accounting/README.md#getpaymentterms)
- [`accountingGetProfile`](docs/sdks/accounting/README.md#getprofile)
- [`accountingGetProjects`](docs/sdks/accounting/README.md#getprojects)
- [`accountingInvoicesUpdateLineItem`](docs/sdks/invoices/README.md#updatelineitem)
- [`accountingJournalEntriesGetAttachments`](docs/sdks/accountingjournalentries/README.md#getattachments)
- [`accountingListBookingProposals`](docs/sdks/accounting/README.md#listbookingproposals)
- [`accountingListCreditNotes`](docs/sdks/accounting/README.md#listcreditnotes)
- [`accountingListJournalEntries`](docs/sdks/accounting/README.md#listjournalentries)
- [`accountingListSalesOrderLineItems`](docs/sdks/accounting/README.md#listsalesorderlineitems)
- [`accountingListSalesOrders`](docs/sdks/accounting/README.md#listsalesorders)
- [`accountingModifyBillLineItem`](docs/sdks/accounting/README.md#modifybilllineitem)
- [`accountingModifySupplier`](docs/sdks/accounting/README.md#modifysupplier)
- [`accountingModifyVendorCredit`](docs/sdks/accounting/README.md#modifyvendorcredit)
- [`accountingRecordTransaction`](docs/sdks/accounting/README.md#recordtransaction)
- [`accountingRemoveBill`](docs/sdks/accounting/README.md#removebill)
- [`accountingRemoveEventSubscription`](docs/sdks/accounting/README.md#removeeventsubscription)
- [`accountingRemovePayment`](docs/sdks/accounting/README.md#removepayment)
- [`accountingReplaceContact`](docs/sdks/accounting/README.md#replacecontact)
- [`accountingRetrieveAccount`](docs/sdks/accounting/README.md#retrieveaccount)
- [`accountingRetrieveAccounts`](docs/sdks/accounting/README.md#retrieveaccounts)
- [`accountingRetrieveBankAccounts`](docs/sdks/accounting/README.md#retrievebankaccounts)
- [`accountingRetrieveBookingProposal`](docs/sdks/accounting/README.md#retrievebookingproposal)
- [`accountingRetrieveDimensions`](docs/sdks/accounting/README.md#retrievedimensions)
- [`accountingRetrieveGoodsReceipt`](docs/sdks/accounting/README.md#retrievegoodsreceipt)
- [`accountingRetrieveGoodsReceiptLineItems`](docs/sdks/accounting/README.md#retrievegoodsreceiptlineitems)
- [`accountingRetrieveInvoiceLineItem`](docs/sdks/accounting/README.md#retrieveinvoicelineitem)
- [`accountingRetrieveInvoiceLineItems`](docs/sdks/accounting/README.md#retrieveinvoicelineitems)
- [`accountingRetrieveInvoices`](docs/sdks/accounting/README.md#retrieveinvoices)
- [`accountingRetrieveItems`](docs/sdks/accounting/README.md#retrieveitems)
- [`accountingRetrieveOfferLineItem`](docs/sdks/accounting/README.md#retrieveofferlineitem)
- [`accountingRetrieveOpenItems`](docs/sdks/accounting/README.md#retrieveopenitems)
- [`accountingRetrievePayments`](docs/sdks/accounting/README.md#retrievepayments)
- [`accountingRetrievePurchaseOrderLineItem`](docs/sdks/accounting/README.md#retrievepurchaseorderlineitem)
- [`accountingRetrievePurchaseOrderLineItems`](docs/sdks/accounting/README.md#retrievepurchaseorderlineitems)
- [`accountingRetrieveSuppliers`](docs/sdks/accounting/README.md#retrievesuppliers)
- [`accountingRetrieveTaxRates`](docs/sdks/accounting/README.md#retrievetaxrates)
- [`accountingRetrieveVendorCredits`](docs/sdks/accounting/README.md#retrievevendorcredits)
- [`accountingUpdateCustomer`](docs/sdks/accounting/README.md#updatecustomer)
- [`accountingUploadFile`](docs/sdks/accounting/README.md#uploadfile)
- [`accountingV2ContactsUpdate`](docs/sdks/v2contacts/README.md#update)
- [`accountingV2CreateBookingProposal`](docs/sdks/accountingv2/README.md#createbookingproposal)
- [`accountingV2CreateContact`](docs/sdks/accountingv2/README.md#createcontact)
- [`accountingV2GetDimension`](docs/sdks/v2/README.md#getdimension)
- [`accountingV2ObtainDimensions`](docs/sdks/accountingv2/README.md#obtaindimensions)
- [`accountingV2UpdateContact`](docs/sdks/accountingv2/README.md#updatecontact)
- [`authApiKeyConfirmation`](docs/sdks/auth/README.md#apikeyconfirmation)
- [`authCallback`](docs/sdks/auth/README.md#callback)
- [`authCancel`](docs/sdks/auth/README.md#cancel)
- [`authCreateEndUserAccount`](docs/sdks/auth/README.md#createenduseraccount)
- [`authGetCompanies`](docs/sdks/auth/README.md#getcompanies)
- [`authGetCompaniesFlow`](docs/sdks/auth/README.md#getcompaniesflow)
- [`authGetEnvironmentPage`](docs/sdks/auth/README.md#getenvironmentpage)
- [`authGetEnvironments`](docs/sdks/auth/README.md#getenvironments)
- [`authGetSubmitPage`](docs/sdks/auth/README.md#getsubmitpage)
- [`authLongToken`](docs/sdks/auth/README.md#longtoken)
- [`authSetEndUserSelections`](docs/sdks/auth/README.md#setenduserselections)
- [`authSystemLoginUrl`](docs/sdks/auth/README.md#systemloginurl)
- [`authTest`](docs/sdks/auth/README.md#test)
- [`billsGetLineItems`](docs/sdks/bills/README.md#getlineitems)
- [`billsUpdate`](docs/sdks/bills/README.md#update)
- [`contactsPatch`](docs/sdks/contacts/README.md#patch)
- [`contactsV2Get`](docs/sdks/contactsv2/README.md#get)
- [`contactsV2List`](docs/sdks/contactsv2/README.md#list)
- [`eventsGetCode`](docs/sdks/events/README.md#getcode)
- [`eventsHandleCallback`](docs/sdks/events/README.md#handlecallback)
- [`eventsHandleConfigurationCallback`](docs/sdks/events/README.md#handleconfigurationcallback)
- [`filesGetDocumentExtensions`](docs/sdks/files/README.md#getdocumentextensions)
- [`fiscalYearsGet`](docs/sdks/fiscalyears/README.md#get)
- [`goodsReceiptsGetLineItem`](docs/sdks/goodsreceipts/README.md#getlineitem)
- [`healthCheck`](docs/sdks/health/README.md#check) - Health check
- [`healthDetails`](docs/sdks/health/README.md#details) - Detailed health check
- [`itemsCreate`](docs/sdks/items/README.md#create)
- [`itemsModify`](docs/sdks/items/README.md#modify)
- [`journalEntriesCreateBulk`](docs/sdks/journalentries/README.md#createbulk)
- [`journalEntryAttachmentsGetById`](docs/sdks/journalentryattachments/README.md#getbyid)
- [`offersGetDocument`](docs/sdks/offers/README.md#getdocument)
- [`purchaseOrdersList`](docs/sdks/purchaseorders/README.md#list)
- [`tenantsAddCallbackUrl`](docs/sdks/tenants/README.md#addcallbackurl)
- [`tenantsCountEndUsersBySystem`](docs/sdks/tenants/README.md#countendusersbysystem)
- [`tenantsDeleteEndUser`](docs/sdks/tenants/README.md#deleteenduser)
- [`tenantsDeleteRegisteredSystem`](docs/sdks/tenants/README.md#deleteregisteredsystem)
- [`tenantsGetAllActiveEndUsers`](docs/sdks/tenants/README.md#getallactiveendusers)
- [`tenantsGetCallbackUrl`](docs/sdks/tenants/README.md#getcallbackurl)
- [`tenantsGetEndUserList`](docs/sdks/tenants/README.md#getenduserlist)
- [`tenantsGetRegisteredSystems`](docs/sdks/tenants/README.md#getregisteredsystems)
- [`tenantsGetRegisteredSystemsMasked`](docs/sdks/tenants/README.md#getregisteredsystemsmasked)
- [`tenantsGetSubmissionPageStyle`](docs/sdks/tenants/README.md#getsubmissionpagestyle)
- [`tenantsGetSubmissionPageStyleByKey`](docs/sdks/tenants/README.md#getsubmissionpagestylebykey)
- [`tenantsGetTargetSystemRequirements`](docs/sdks/tenants/README.md#gettargetsystemrequirements)
- [`tenantsGetTargetSystemValues`](docs/sdks/tenants/README.md#gettargetsystemvalues)
- [`tenantsSystemRegistration`](docs/sdks/tenants/README.md#systemregistration)
- [`tenantsUpdateSubmissionPageStyle`](docs/sdks/tenants/README.md#updatesubmissionpagestyle)
- [`userGetInfo`](docs/sdks/user/README.md#getinfo)
- [`vendorCreditsDelete`](docs/sdks/vendorcredits/README.md#delete)
- [`webhooksCreateWebhook`](docs/sdks/webhooks/README.md#createwebhook)
- [`webhooksCreateWebhookConfig`](docs/sdks/webhooks/README.md#createwebhookconfig)
- [`webhooksCreateWebhookEndUser`](docs/sdks/webhooks/README.md#createwebhookenduser)
- [`webhooksCreateWebHookTenant`](docs/sdks/webhooks/README.md#createwebhooktenant)
- [`webhooksDeleteWebhook`](docs/sdks/webhooks/README.md#deletewebhook)
- [`webhooksDeleteWebhookEndUser`](docs/sdks/webhooks/README.md#deletewebhookenduser)
- [`webhooksDeleteWebhookTenant`](docs/sdks/webhooks/README.md#deletewebhooktenant)
- [`webhooksGetWebhooks`](docs/sdks/webhooks/README.md#getwebhooks)

</details>
<!-- End Standalone functions [standalone-funcs] -->

<!-- Start File uploads [file-upload] -->
## File uploads

Certain SDK methods accept files as part of a multi-part request. It is possible and typically recommended to upload files as a stream rather than reading the entire contents into memory. This avoids excessive memory consumption and potentially crashing with out-of-memory errors when working with very large files. The following example demonstrates how to attach a file stream to a request.

> [!TIP]
>
> Depending on your JavaScript runtime, there are convenient utilities that return a handle to a file without reading the entire contents into memory:
>
> - **Node.js v20+:** Since v20, Node.js comes with a native `openAsBlob` function in [`node:fs`](https://nodejs.org/docs/latest-v20.x/api/fs.html#fsopenasblobpath-options).
> - **Bun:** The native [`Bun.file`](https://bun.sh/docs/api/file-io#reading-files-bun-file) function produces a file handle that can be used for streaming file uploads.
> - **Browsers:** All supported browsers return an instance to a [`File`](https://developer.mozilla.org/en-US/docs/Web/API/File) when reading the value from an `<input type="file">` element.
> - **Node.js v18:** A file stream can be created using the `fileFrom` helper from [`fetch-blob/from.js`](https://www.npmjs.com/package/fetch-blob).

```typescript
import { Maesn } from "@maesn/typescript-sdk";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
  security: {
    apiKey: process.env["MAESN_API_KEY"] ?? "",
    accountKey: process.env["MAESN_ACCOUNT_KEY"] ?? "",
  },
});

async function run() {
  const result = await maesn.accounting.recordTransaction({
    body: {},
  });

  console.log(result);
}

run();

```
<!-- End File uploads [file-upload] -->

<!-- Start Retries [retries] -->
## Retries

Some of the endpoints in this SDK support retries.  If you use the SDK without any configuration, it will fall back to the default retry strategy provided by the API.  However, the default retry strategy can be overridden on a per-operation basis, or across the entire SDK.

To change the default retry strategy for a single API call, simply provide a retryConfig object to the call:
```typescript
import { Maesn } from "@maesn/typescript-sdk";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
  security: {
    apiKey: process.env["MAESN_API_KEY"] ?? "",
    accountKey: process.env["MAESN_ACCOUNT_KEY"] ?? "",
  },
});

async function run() {
  const result = await maesn.accounting.retrieveAccount({
    accountId: "<id>",
  }, {
    retries: {
      strategy: "backoff",
      backoff: {
        initialInterval: 1,
        maxInterval: 50,
        exponent: 1.1,
        maxElapsedTime: 100,
      },
      retryConnectionErrors: false,
    },
  });

  console.log(result);
}

run();

```

If you'd like to override the default retry strategy for all operations that support retries, you can provide a retryConfig at SDK initialization:
```typescript
import { Maesn } from "@maesn/typescript-sdk";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
  retryConfig: {
    strategy: "backoff",
    backoff: {
      initialInterval: 1,
      maxInterval: 50,
      exponent: 1.1,
      maxElapsedTime: 100,
    },
    retryConnectionErrors: false,
  },
  security: {
    apiKey: process.env["MAESN_API_KEY"] ?? "",
    accountKey: process.env["MAESN_ACCOUNT_KEY"] ?? "",
  },
});

async function run() {
  const result = await maesn.accounting.retrieveAccount({
    accountId: "<id>",
  });

  console.log(result);
}

run();

```
<!-- End Retries [retries] -->

<!-- Start Error Handling [errors] -->
## Error Handling

[`MaesnError`](./src/models/errors/maesn-error.ts) is the base class for all HTTP error responses. It has the following properties:

| Property            | Type       | Description                                                                             |
| ------------------- | ---------- | --------------------------------------------------------------------------------------- |
| `error.message`     | `string`   | Error message                                                                           |
| `error.statusCode`  | `number`   | HTTP response status code eg `404`                                                      |
| `error.headers`     | `Headers`  | HTTP response headers                                                                   |
| `error.body`        | `string`   | HTTP body. Can be empty string if no body is returned.                                  |
| `error.rawResponse` | `Response` | Raw HTTP response                                                                       |
| `error.data$`       |            | Optional. Some errors may contain structured data. [See Error Classes](#error-classes). |

### Example
```typescript
import { Maesn } from "@maesn/typescript-sdk";
import * as errors from "@maesn/typescript-sdk/models/errors";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
  security: {
    apiKey: process.env["MAESN_API_KEY"] ?? "",
    accountKey: process.env["MAESN_ACCOUNT_KEY"] ?? "",
  },
});

async function run() {
  try {
    const result = await maesn.health.details();

    console.log(result);
  } catch (error) {
    // The base class for HTTP error responses
    if (error instanceof errors.MaesnError) {
      console.log(error.message);
      console.log(error.statusCode);
      console.log(error.body);
      console.log(error.headers);

      // Depending on the method different errors may be thrown
      if (error instanceof errors.ServiceUnavailableError) {
        console.log(error.data$.status); // string
        console.log(error.data$.info); // { [k: string]: Info }
        console.log(error.data$.error); // { [k: string]: ErrorT }
        console.log(error.data$.details); // { [k: string]: Details }
      }
    }
  }
}

run();

```

### Error Classes
**Primary error:**
* [`MaesnError`](./src/models/errors/maesn-error.ts): The base class for HTTP error responses.

<details><summary>Less common errors (7)</summary>

<br />

**Network errors:**
* [`ConnectionError`](./src/models/errors/http-client-errors.ts): HTTP client was unable to make a request to a server.
* [`RequestTimeoutError`](./src/models/errors/http-client-errors.ts): HTTP request timed out due to an AbortSignal signal.
* [`RequestAbortedError`](./src/models/errors/http-client-errors.ts): HTTP request was aborted by the client.
* [`InvalidRequestError`](./src/models/errors/http-client-errors.ts): Any input used to create a request is invalid.
* [`UnexpectedClientError`](./src/models/errors/http-client-errors.ts): Unrecognised or unexpected error.


**Inherit from [`MaesnError`](./src/models/errors/maesn-error.ts)**:
* [`ServiceUnavailableError`](./src/models/errors/service-unavailable-error.ts): The Health Check is not successful. Status code `503`. Applicable to 1 of 162 methods.*
* [`ResponseValidationError`](./src/models/errors/response-validation-error.ts): Type mismatch between the data returned from the server and the structure expected by the SDK. See `error.rawValue` for the raw value and `error.pretty()` for a nicely formatted multi-line string.

</details>

\* Check [the method documentation](#available-resources-and-operations) to see if the error is applicable.
<!-- End Error Handling [errors] -->

<!-- Start Custom HTTP Client [http-client] -->
## Custom HTTP Client

The TypeScript SDK makes API calls using an `HTTPClient` that wraps the native
[Fetch API](https://developer.mozilla.org/en-US/docs/Web/API/Fetch_API). This
client is a thin wrapper around `fetch` and provides the ability to attach hooks
around the request lifecycle that can be used to modify the request or handle
errors and response.

The `HTTPClient` constructor takes an optional `fetcher` argument that can be
used to integrate a third-party HTTP client or when writing tests to mock out
the HTTP client and feed in fixtures.

The following example shows how to:
- route requests through a proxy server using [undici](https://www.npmjs.com/package/undici)'s ProxyAgent
- use the `"beforeRequest"` hook to add a custom header and a timeout to requests
- use the `"requestError"` hook to log errors

```typescript
import { Maesn } from "@maesn/typescript-sdk";
import { ProxyAgent } from "undici";
import { HTTPClient } from "@maesn/typescript-sdk/lib/http";

const dispatcher = new ProxyAgent("http://proxy.example.com:8080");

const httpClient = new HTTPClient({
  // 'fetcher' takes a function that has the same signature as native 'fetch'.
  fetcher: (input, init) =>
    // 'dispatcher' is specific to undici and not part of the standard Fetch API.
    fetch(input, { ...init, dispatcher } as RequestInit),
});

httpClient.addHook("beforeRequest", (request) => {
  const nextRequest = new Request(request, {
    signal: request.signal || AbortSignal.timeout(5000)
  });

  nextRequest.headers.set("x-custom-header", "custom value");

  return nextRequest;
});

httpClient.addHook("requestError", (error, request) => {
  console.group("Request Error");
  console.log("Reason:", `${error}`);
  console.log("Endpoint:", `${request.method} ${request.url}`);
  console.groupEnd();
});

const sdk = new Maesn({ httpClient: httpClient });
```
<!-- End Custom HTTP Client [http-client] -->

<!-- Start Debugging [debug] -->
## Debugging

You can setup your SDK to emit debug logs for SDK requests and responses.

You can pass a logger that matches `console`'s interface as an SDK option.

> [!WARNING]
> Beware that debug logging will reveal secrets, like API tokens in headers, in log messages printed to a console or files. It's recommended to use this feature only during local development and not in production.

```typescript
import { Maesn } from "@maesn/typescript-sdk";

const sdk = new Maesn({ debugLogger: console });
```

You can also enable a default debug logger by setting an environment variable `MAESN_DEBUG` to true.
<!-- End Debugging [debug] -->

<!-- Placeholder for Future Speakeasy SDK Sections -->

# Development

## Maturity

This SDK is in beta, and there may be breaking changes between versions without a major version update. Therefore, we recommend pinning usage
to a specific package version. This way, you can install the same version each time without breaking changes unless you are intentionally
looking for the latest version.

## Contributions

While we value open-source contributions to this SDK, this library is generated programmatically. Any manual changes added to internal files will be overwritten on the next generation. 
We look forward to hearing your feedback. Feel free to open a PR or an issue with a proof of concept and we'll do our best to include it in a future release. 

### SDK Created by [Speakeasy](https://www.speakeasy.com/?utm_source=maesn&utm_campaign=typescript)
