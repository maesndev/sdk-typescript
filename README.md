# maesn

Developer-friendly & type-safe Typescript SDK specifically catered to leverage *maesn* API.

[![Built by Speakeasy](https://img.shields.io/badge/Built_by-SPEAKEASY-374151?style=for-the-badge&labelColor=f3f4f6)](https://www.speakeasy.com/?utm_source=maesn&utm_campaign=typescript)
[![License: MIT](https://img.shields.io/badge/LICENSE_//_MIT-3b5bdb?style=for-the-badge&labelColor=eff6ff)](https://opensource.org/licenses/MIT)


<!-- Start Summary [summary] -->
## Summary

Maesn Unified API: Maesn is the only Unified API that provides standard endpoints tailored for ERP use cases. We will continuously work on improving and extending our portfolio of use cases and ERP systems that we offer easy integration to.

Beside great use-cases, the most relevant ERP systems and the best possible support, we provide several technical key features that enable you to accelerate your integration game:

- Drop-in frontend authentication components that makes it easy to connect to your customers’ end systems.
- Authenticated pass through request for the occasional API endpoint not included in our common data models.
- Templates for you docs, so that you have all content for your end user-onboarding ready

Once you get started with maesn and integrate with our endpoints, you automatically have support for all existing and new integrations we add.
<!-- End Summary [summary] -->

<!-- Start Table of Contents [toc] -->
## Table of Contents
<!-- $toc-max-depth=2 -->
* [maesn](#maesn)
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
  const result = await maesn.accounting.getAccount({
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
  const result = await maesn.accounting.getAccount({
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

* [getAccount](docs/sdks/accounting/README.md#getaccount)
* [getAccounts](docs/sdks/accounting/README.md#getaccounts)
* [createAccount](docs/sdks/accounting/README.md#createaccount)
* [getBankAccounts](docs/sdks/accounting/README.md#getbankaccounts)
* [createBankAccount](docs/sdks/accounting/README.md#createbankaccount)
* [getBankAccount](docs/sdks/accounting/README.md#getbankaccount)
* [getDimensions](docs/sdks/accounting/README.md#getdimensions)
* [createTransaction](docs/sdks/accounting/README.md#createtransaction)
* [getCustomers](docs/sdks/accounting/README.md#getcustomers)
* [createCustomer](docs/sdks/accounting/README.md#createcustomer)
* [getCustomer](docs/sdks/accounting/README.md#getcustomer)
* [updateCustomer](docs/sdks/accounting/README.md#updatecustomer)
* [patchCustomers](docs/sdks/accounting/README.md#patchcustomers)
* [getSuppliers](docs/sdks/accounting/README.md#getsuppliers)
* [createSupplier](docs/sdks/accounting/README.md#createsupplier)
* [getSupplier](docs/sdks/accounting/README.md#getsupplier)
* [updateSupplier](docs/sdks/accounting/README.md#updatesupplier)
* [patchSupplier](docs/sdks/accounting/README.md#patchsupplier)
* [getContacts](docs/sdks/accounting/README.md#getcontacts)
* [createContact](docs/sdks/accounting/README.md#createcontact)
* [getContact](docs/sdks/accounting/README.md#getcontact)
* [putContact](docs/sdks/accounting/README.md#putcontact)
* [patchContact](docs/sdks/accounting/README.md#patchcontact)
* [createContacts](docs/sdks/accounting/README.md#createcontacts)
* [createContactsV1](docs/sdks/accounting/README.md#createcontactsv1)
* [getInvoices](docs/sdks/accounting/README.md#getinvoices)
* [createInvoice](docs/sdks/accounting/README.md#createinvoice)
* [getInvoice](docs/sdks/accounting/README.md#getinvoice)
* [patchInvoice](docs/sdks/accounting/README.md#patchinvoice)
* [getInvoiceDocument](docs/sdks/accounting/README.md#getinvoicedocument)
* [postFile](docs/sdks/accounting/README.md#postfile)
* [getDocumentTypes](docs/sdks/accounting/README.md#getdocumenttypes)
* [getDocumentExtensions](docs/sdks/accounting/README.md#getdocumentextensions)
* [getAsyncTaskInfo](docs/sdks/accounting/README.md#getasynctaskinfo)
* [getItems](docs/sdks/accounting/README.md#getitems)
* [createItem](docs/sdks/accounting/README.md#createitem)
* [getItem](docs/sdks/accounting/README.md#getitem)
* [patchItem](docs/sdks/accounting/README.md#patchitem)
* [getLineItems](docs/sdks/accounting/README.md#getlineitems)
* [createLineItem](docs/sdks/accounting/README.md#createlineitem)
* [getLineItem](docs/sdks/accounting/README.md#getlineitem)
* [patchLineItem](docs/sdks/accounting/README.md#patchlineitem)
* [getJournals](docs/sdks/accounting/README.md#getjournals)
* [getJournalEntries](docs/sdks/accounting/README.md#getjournalentries)
* [createJournalEntry](docs/sdks/accounting/README.md#createjournalentry)
* [getJournalEntry](docs/sdks/accounting/README.md#getjournalentry)
* [createJournalEntries](docs/sdks/accounting/README.md#createjournalentries)
* [getJournalEntryAttachments](docs/sdks/accounting/README.md#getjournalentryattachments)
* [createJournalEntryAttachments](docs/sdks/accounting/README.md#createjournalentryattachments)
* [getJournalEntryAttachmentById](docs/sdks/accounting/README.md#getjournalentryattachmentbyid)
* [getOffers](docs/sdks/accounting/README.md#getoffers)
* [createOffer](docs/sdks/accounting/README.md#createoffer)
* [getOffer](docs/sdks/accounting/README.md#getoffer)
* [getOfferLineItems](docs/sdks/accounting/README.md#getofferlineitems)
* [getOfferLineItem](docs/sdks/accounting/README.md#getofferlineitem)
* [getOfferDocument](docs/sdks/accounting/README.md#getofferdocument)
* [createExpense](docs/sdks/accounting/README.md#createexpense)
* [getExpenses](docs/sdks/accounting/README.md#getexpenses)
* [getExpense](docs/sdks/accounting/README.md#getexpense)
* [getProjects](docs/sdks/accounting/README.md#getprojects)
* [createProject](docs/sdks/accounting/README.md#createproject)
* [getProject](docs/sdks/accounting/README.md#getproject)
* [getSalesOrders](docs/sdks/accounting/README.md#getsalesorders)
* [createSalesOrder](docs/sdks/accounting/README.md#createsalesorder)
* [getSalesOrder](docs/sdks/accounting/README.md#getsalesorder)
* [getSalesOrderLines](docs/sdks/accounting/README.md#getsalesorderlines)
* [getPaymentTerms](docs/sdks/accounting/README.md#getpaymentterms)
* [createPaymentTerm](docs/sdks/accounting/README.md#createpaymentterm)
* [getPaymentTerm](docs/sdks/accounting/README.md#getpaymentterm)
* [getTaxRates](docs/sdks/accounting/README.md#gettaxrates)
* [getTaxRate](docs/sdks/accounting/README.md#gettaxrate)
* [getPayments](docs/sdks/accounting/README.md#getpayments)
* [createPayment](docs/sdks/accounting/README.md#createpayment)
* [getPayment](docs/sdks/accounting/README.md#getpayment)
* [deletePayment](docs/sdks/accounting/README.md#deletepayment)
* [createEventSubscriptions](docs/sdks/accounting/README.md#createeventsubscriptions)
* [deleteEventSubscriptions](docs/sdks/accounting/README.md#deleteeventsubscriptions)
* [getProfile](docs/sdks/accounting/README.md#getprofile)
* [createPassThroughRequest](docs/sdks/accounting/README.md#createpassthroughrequest)
* [getBills](docs/sdks/accounting/README.md#getbills)
* [createBill](docs/sdks/accounting/README.md#createbill)
* [getBill](docs/sdks/accounting/README.md#getbill)
* [updateBill](docs/sdks/accounting/README.md#updatebill)
* [deleteBill](docs/sdks/accounting/README.md#deletebill)
* [getBillDocument](docs/sdks/accounting/README.md#getbilldocument)
* [createBookingProposal](docs/sdks/accounting/README.md#createbookingproposal)
* [getBookingProposals](docs/sdks/accounting/README.md#getbookingproposals)
* [getBookingProposal](docs/sdks/accounting/README.md#getbookingproposal)
* [getBookingProposalDocument](docs/sdks/accounting/README.md#getbookingproposaldocument)
* [getVendorCredits](docs/sdks/accounting/README.md#getvendorcredits)
* [createVendorCredit](docs/sdks/accounting/README.md#createvendorcredit)
* [updateVendorCredit](docs/sdks/accounting/README.md#updatevendorcredit)
* [deleteVendorCredit](docs/sdks/accounting/README.md#deletevendorcredit)
* [getBillLineItems](docs/sdks/accounting/README.md#getbilllineitems)
* [createBillLineItem](docs/sdks/accounting/README.md#createbilllineitem)
* [updateBillLineItem](docs/sdks/accounting/README.md#updatebilllineitem)
* [getPurchaseOrders](docs/sdks/accounting/README.md#getpurchaseorders)
* [getPurchaseOrder](docs/sdks/accounting/README.md#getpurchaseorder)
* [getPurchaseOrderLineItems](docs/sdks/accounting/README.md#getpurchaseorderlineitems)
* [getPurchaseOrderLineItem](docs/sdks/accounting/README.md#getpurchaseorderlineitem)
* [getGoodsReceipts](docs/sdks/accounting/README.md#getgoodsreceipts)
* [getGoodsReceipt](docs/sdks/accounting/README.md#getgoodsreceipt)
* [getGoodsReceiptLineItems](docs/sdks/accounting/README.md#getgoodsreceiptlineitems)
* [getGoodsReceiptLineItem](docs/sdks/accounting/README.md#getgoodsreceiptlineitem)
* [getUnits](docs/sdks/accounting/README.md#getunits)
* [getOpenItems](docs/sdks/accounting/README.md#getopenitems)
* [getTrialBalance](docs/sdks/accounting/README.md#gettrialbalance)
* [getCreditNotes](docs/sdks/accounting/README.md#getcreditnotes)
* [getCreditNote](docs/sdks/accounting/README.md#getcreditnote)
* [getFiscalYears](docs/sdks/accounting/README.md#getfiscalyears)
* [getFiscalYear](docs/sdks/accounting/README.md#getfiscalyear)

### [AccountingV2](docs/sdks/accountingv2/README.md)

* [createBookingProposalV2](docs/sdks/accountingv2/README.md#createbookingproposalv2)
* [getContactsV2](docs/sdks/accountingv2/README.md#getcontactsv2)
* [createContactV2](docs/sdks/accountingv2/README.md#createcontactv2)
* [getContactV2](docs/sdks/accountingv2/README.md#getcontactv2)
* [putContactV2](docs/sdks/accountingv2/README.md#putcontactv2)
* [patchContactV2](docs/sdks/accountingv2/README.md#patchcontactv2)
* [getDimensionsV2](docs/sdks/accountingv2/README.md#getdimensionsv2)
* [getDimensionsByDimension](docs/sdks/accountingv2/README.md#getdimensionsbydimension)

### [Auth](docs/sdks/auth/README.md)

* [getEnvironments](docs/sdks/auth/README.md#getenvironments)
* [getCompanies](docs/sdks/auth/README.md#getcompanies)
* [systemLoginUrl](docs/sdks/auth/README.md#systemloginurl)
* [createEndUserAccount](docs/sdks/auth/README.md#createenduseraccount)

### [Events](docs/sdks/events/README.md)

* [handleCallback](docs/sdks/events/README.md#handlecallback)
* [getCode](docs/sdks/events/README.md#getcode)
* [handleConfigurationCallback](docs/sdks/events/README.md#handleconfigurationcallback)

### [Health](docs/sdks/health/README.md)

* [check](docs/sdks/health/README.md#check) - Health check

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
* [getSubmissionPageStyle](docs/sdks/tenants/README.md#getsubmissionpagestyle)
* [updateSubmissionPageStyle](docs/sdks/tenants/README.md#updatesubmissionpagestyle)
* [getSubmissionPageStyleByKey](docs/sdks/tenants/README.md#getsubmissionpagestylebykey)

### [User](docs/sdks/user/README.md)

* [getUserInfo](docs/sdks/user/README.md#getuserinfo)

### [Webhooks](docs/sdks/webhooks/README.md)

* [createWebhookEndUser](docs/sdks/webhooks/README.md#createwebhookenduser)
* [deleteWebhookEndUser](docs/sdks/webhooks/README.md#deletewebhookenduser)
* [createWebhook](docs/sdks/webhooks/README.md#createwebhook)
* [getWebhooks](docs/sdks/webhooks/README.md#getwebhooks)
* [deleteWebhook](docs/sdks/webhooks/README.md#deletewebhook)

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

- [`accountingCreateAccount`](docs/sdks/accounting/README.md#createaccount)
- [`accountingCreateBankAccount`](docs/sdks/accounting/README.md#createbankaccount)
- [`accountingCreateBill`](docs/sdks/accounting/README.md#createbill)
- [`accountingCreateBillLineItem`](docs/sdks/accounting/README.md#createbilllineitem)
- [`accountingCreateBookingProposal`](docs/sdks/accounting/README.md#createbookingproposal)
- [`accountingCreateContact`](docs/sdks/accounting/README.md#createcontact)
- [`accountingCreateContacts`](docs/sdks/accounting/README.md#createcontacts)
- [`accountingCreateContactsV1`](docs/sdks/accounting/README.md#createcontactsv1)
- [`accountingCreateCustomer`](docs/sdks/accounting/README.md#createcustomer)
- [`accountingCreateEventSubscriptions`](docs/sdks/accounting/README.md#createeventsubscriptions)
- [`accountingCreateExpense`](docs/sdks/accounting/README.md#createexpense)
- [`accountingCreateInvoice`](docs/sdks/accounting/README.md#createinvoice)
- [`accountingCreateItem`](docs/sdks/accounting/README.md#createitem)
- [`accountingCreateJournalEntries`](docs/sdks/accounting/README.md#createjournalentries)
- [`accountingCreateJournalEntry`](docs/sdks/accounting/README.md#createjournalentry)
- [`accountingCreateJournalEntryAttachments`](docs/sdks/accounting/README.md#createjournalentryattachments)
- [`accountingCreateLineItem`](docs/sdks/accounting/README.md#createlineitem)
- [`accountingCreateOffer`](docs/sdks/accounting/README.md#createoffer)
- [`accountingCreatePassThroughRequest`](docs/sdks/accounting/README.md#createpassthroughrequest)
- [`accountingCreatePayment`](docs/sdks/accounting/README.md#createpayment)
- [`accountingCreatePaymentTerm`](docs/sdks/accounting/README.md#createpaymentterm)
- [`accountingCreateProject`](docs/sdks/accounting/README.md#createproject)
- [`accountingCreateSalesOrder`](docs/sdks/accounting/README.md#createsalesorder)
- [`accountingCreateSupplier`](docs/sdks/accounting/README.md#createsupplier)
- [`accountingCreateTransaction`](docs/sdks/accounting/README.md#createtransaction)
- [`accountingCreateVendorCredit`](docs/sdks/accounting/README.md#createvendorcredit)
- [`accountingDeleteBill`](docs/sdks/accounting/README.md#deletebill)
- [`accountingDeleteEventSubscriptions`](docs/sdks/accounting/README.md#deleteeventsubscriptions)
- [`accountingDeletePayment`](docs/sdks/accounting/README.md#deletepayment)
- [`accountingDeleteVendorCredit`](docs/sdks/accounting/README.md#deletevendorcredit)
- [`accountingGetAccount`](docs/sdks/accounting/README.md#getaccount)
- [`accountingGetAccounts`](docs/sdks/accounting/README.md#getaccounts)
- [`accountingGetAsyncTaskInfo`](docs/sdks/accounting/README.md#getasynctaskinfo)
- [`accountingGetBankAccount`](docs/sdks/accounting/README.md#getbankaccount)
- [`accountingGetBankAccounts`](docs/sdks/accounting/README.md#getbankaccounts)
- [`accountingGetBill`](docs/sdks/accounting/README.md#getbill)
- [`accountingGetBillDocument`](docs/sdks/accounting/README.md#getbilldocument)
- [`accountingGetBillLineItems`](docs/sdks/accounting/README.md#getbilllineitems)
- [`accountingGetBills`](docs/sdks/accounting/README.md#getbills)
- [`accountingGetBookingProposal`](docs/sdks/accounting/README.md#getbookingproposal)
- [`accountingGetBookingProposalDocument`](docs/sdks/accounting/README.md#getbookingproposaldocument)
- [`accountingGetBookingProposals`](docs/sdks/accounting/README.md#getbookingproposals)
- [`accountingGetContact`](docs/sdks/accounting/README.md#getcontact)
- [`accountingGetContacts`](docs/sdks/accounting/README.md#getcontacts)
- [`accountingGetCreditNote`](docs/sdks/accounting/README.md#getcreditnote)
- [`accountingGetCreditNotes`](docs/sdks/accounting/README.md#getcreditnotes)
- [`accountingGetCustomer`](docs/sdks/accounting/README.md#getcustomer)
- [`accountingGetCustomers`](docs/sdks/accounting/README.md#getcustomers)
- [`accountingGetDimensions`](docs/sdks/accounting/README.md#getdimensions)
- [`accountingGetDocumentExtensions`](docs/sdks/accounting/README.md#getdocumentextensions)
- [`accountingGetDocumentTypes`](docs/sdks/accounting/README.md#getdocumenttypes)
- [`accountingGetExpense`](docs/sdks/accounting/README.md#getexpense)
- [`accountingGetExpenses`](docs/sdks/accounting/README.md#getexpenses)
- [`accountingGetFiscalYear`](docs/sdks/accounting/README.md#getfiscalyear)
- [`accountingGetFiscalYears`](docs/sdks/accounting/README.md#getfiscalyears)
- [`accountingGetGoodsReceipt`](docs/sdks/accounting/README.md#getgoodsreceipt)
- [`accountingGetGoodsReceiptLineItem`](docs/sdks/accounting/README.md#getgoodsreceiptlineitem)
- [`accountingGetGoodsReceiptLineItems`](docs/sdks/accounting/README.md#getgoodsreceiptlineitems)
- [`accountingGetGoodsReceipts`](docs/sdks/accounting/README.md#getgoodsreceipts)
- [`accountingGetInvoice`](docs/sdks/accounting/README.md#getinvoice)
- [`accountingGetInvoiceDocument`](docs/sdks/accounting/README.md#getinvoicedocument)
- [`accountingGetInvoices`](docs/sdks/accounting/README.md#getinvoices)
- [`accountingGetItem`](docs/sdks/accounting/README.md#getitem)
- [`accountingGetItems`](docs/sdks/accounting/README.md#getitems)
- [`accountingGetJournalEntries`](docs/sdks/accounting/README.md#getjournalentries)
- [`accountingGetJournalEntry`](docs/sdks/accounting/README.md#getjournalentry)
- [`accountingGetJournalEntryAttachmentById`](docs/sdks/accounting/README.md#getjournalentryattachmentbyid)
- [`accountingGetJournalEntryAttachments`](docs/sdks/accounting/README.md#getjournalentryattachments)
- [`accountingGetJournals`](docs/sdks/accounting/README.md#getjournals)
- [`accountingGetLineItem`](docs/sdks/accounting/README.md#getlineitem)
- [`accountingGetLineItems`](docs/sdks/accounting/README.md#getlineitems)
- [`accountingGetOffer`](docs/sdks/accounting/README.md#getoffer)
- [`accountingGetOfferDocument`](docs/sdks/accounting/README.md#getofferdocument)
- [`accountingGetOfferLineItem`](docs/sdks/accounting/README.md#getofferlineitem)
- [`accountingGetOfferLineItems`](docs/sdks/accounting/README.md#getofferlineitems)
- [`accountingGetOffers`](docs/sdks/accounting/README.md#getoffers)
- [`accountingGetOpenItems`](docs/sdks/accounting/README.md#getopenitems)
- [`accountingGetPayment`](docs/sdks/accounting/README.md#getpayment)
- [`accountingGetPayments`](docs/sdks/accounting/README.md#getpayments)
- [`accountingGetPaymentTerm`](docs/sdks/accounting/README.md#getpaymentterm)
- [`accountingGetPaymentTerms`](docs/sdks/accounting/README.md#getpaymentterms)
- [`accountingGetProfile`](docs/sdks/accounting/README.md#getprofile)
- [`accountingGetProject`](docs/sdks/accounting/README.md#getproject)
- [`accountingGetProjects`](docs/sdks/accounting/README.md#getprojects)
- [`accountingGetPurchaseOrder`](docs/sdks/accounting/README.md#getpurchaseorder)
- [`accountingGetPurchaseOrderLineItem`](docs/sdks/accounting/README.md#getpurchaseorderlineitem)
- [`accountingGetPurchaseOrderLineItems`](docs/sdks/accounting/README.md#getpurchaseorderlineitems)
- [`accountingGetPurchaseOrders`](docs/sdks/accounting/README.md#getpurchaseorders)
- [`accountingGetSalesOrder`](docs/sdks/accounting/README.md#getsalesorder)
- [`accountingGetSalesOrderLines`](docs/sdks/accounting/README.md#getsalesorderlines)
- [`accountingGetSalesOrders`](docs/sdks/accounting/README.md#getsalesorders)
- [`accountingGetSupplier`](docs/sdks/accounting/README.md#getsupplier)
- [`accountingGetSuppliers`](docs/sdks/accounting/README.md#getsuppliers)
- [`accountingGetTaxRate`](docs/sdks/accounting/README.md#gettaxrate)
- [`accountingGetTaxRates`](docs/sdks/accounting/README.md#gettaxrates)
- [`accountingGetTrialBalance`](docs/sdks/accounting/README.md#gettrialbalance)
- [`accountingGetUnits`](docs/sdks/accounting/README.md#getunits)
- [`accountingGetVendorCredits`](docs/sdks/accounting/README.md#getvendorcredits)
- [`accountingPatchContact`](docs/sdks/accounting/README.md#patchcontact)
- [`accountingPatchCustomers`](docs/sdks/accounting/README.md#patchcustomers)
- [`accountingPatchInvoice`](docs/sdks/accounting/README.md#patchinvoice)
- [`accountingPatchItem`](docs/sdks/accounting/README.md#patchitem)
- [`accountingPatchLineItem`](docs/sdks/accounting/README.md#patchlineitem)
- [`accountingPatchSupplier`](docs/sdks/accounting/README.md#patchsupplier)
- [`accountingPostFile`](docs/sdks/accounting/README.md#postfile)
- [`accountingPutContact`](docs/sdks/accounting/README.md#putcontact)
- [`accountingUpdateBill`](docs/sdks/accounting/README.md#updatebill)
- [`accountingUpdateBillLineItem`](docs/sdks/accounting/README.md#updatebilllineitem)
- [`accountingUpdateCustomer`](docs/sdks/accounting/README.md#updatecustomer)
- [`accountingUpdateSupplier`](docs/sdks/accounting/README.md#updatesupplier)
- [`accountingUpdateVendorCredit`](docs/sdks/accounting/README.md#updatevendorcredit)
- [`accountingV2CreateBookingProposalV2`](docs/sdks/accountingv2/README.md#createbookingproposalv2)
- [`accountingV2CreateContactV2`](docs/sdks/accountingv2/README.md#createcontactv2)
- [`accountingV2GetContactsV2`](docs/sdks/accountingv2/README.md#getcontactsv2)
- [`accountingV2GetContactV2`](docs/sdks/accountingv2/README.md#getcontactv2)
- [`accountingV2GetDimensionsByDimension`](docs/sdks/accountingv2/README.md#getdimensionsbydimension)
- [`accountingV2GetDimensionsV2`](docs/sdks/accountingv2/README.md#getdimensionsv2)
- [`accountingV2PatchContactV2`](docs/sdks/accountingv2/README.md#patchcontactv2)
- [`accountingV2PutContactV2`](docs/sdks/accountingv2/README.md#putcontactv2)
- [`authCreateEndUserAccount`](docs/sdks/auth/README.md#createenduseraccount)
- [`authGetCompanies`](docs/sdks/auth/README.md#getcompanies)
- [`authGetEnvironments`](docs/sdks/auth/README.md#getenvironments)
- [`authSystemLoginUrl`](docs/sdks/auth/README.md#systemloginurl)
- [`eventsGetCode`](docs/sdks/events/README.md#getcode)
- [`eventsHandleCallback`](docs/sdks/events/README.md#handlecallback)
- [`eventsHandleConfigurationCallback`](docs/sdks/events/README.md#handleconfigurationcallback)
- [`healthCheck`](docs/sdks/health/README.md#check) - Health check
- [`tenantsAddCallbackUrl`](docs/sdks/tenants/README.md#addcallbackurl)
- [`tenantsCountEndUsersBySystem`](docs/sdks/tenants/README.md#countendusersbysystem)
- [`tenantsDeleteEndUser`](docs/sdks/tenants/README.md#deleteenduser)
- [`tenantsDeleteRegisteredSystem`](docs/sdks/tenants/README.md#deleteregisteredsystem)
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
- [`userGetUserInfo`](docs/sdks/user/README.md#getuserinfo)
- [`webhooksCreateWebhook`](docs/sdks/webhooks/README.md#createwebhook)
- [`webhooksCreateWebhookEndUser`](docs/sdks/webhooks/README.md#createwebhookenduser)
- [`webhooksDeleteWebhook`](docs/sdks/webhooks/README.md#deletewebhook)
- [`webhooksDeleteWebhookEndUser`](docs/sdks/webhooks/README.md#deletewebhookenduser)
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
  const result = await maesn.accounting.createTransaction({
    body: {},
  });

  console.log(result);
}

run();

```
<!-- End File uploads [file-upload] -->

## Retries

All **GET** endpoints automatically retry on `5XX` errors and connection failures using exponential backoff. **POST, PUT, PATCH, and DELETE** endpoints never retry automatically to avoid creating duplicate records.

Default retry configuration:

| Parameter | Value |
|---|---|
| Strategy | Exponential backoff |
| Initial interval | 500 ms |
| Max interval | 60 s |
| Exponent | 1.5 |
| Max elapsed time | 1 h |
| Retried status codes | 5XX |
| Retry connection errors | Yes |

You can override the retry strategy per call:
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
  const result = await maesn.accounting.getAccount({
    accountId: "<id>",
  }, {
    retries: {
      strategy: "backoff",
      backoff: {
        initialInterval: 500,
        maxInterval: 60000,
        exponent: 1.5,
        maxElapsedTime: 3600000,
      },
      retryConnectionErrors: true,
    },
  });

  console.log(result);
}

run();

```

Or override the default for all operations at SDK initialization:
```typescript
import { Maesn } from "@maesn/typescript-sdk";

const maesn = new Maesn({
  serverURL: "https://api.example.com",
  retryConfig: {
    strategy: "backoff",
    backoff: {
      initialInterval: 500,
      maxInterval: 60000,
      exponent: 1.5,
      maxElapsedTime: 3600000,
    },
    retryConnectionErrors: true,
  },
  security: {
    apiKey: process.env["MAESN_API_KEY"] ?? "",
    accountKey: process.env["MAESN_ACCOUNT_KEY"] ?? "",
  },
});

async function run() {
  const result = await maesn.accounting.getAccount({
    accountId: "<id>",
  });

  console.log(result);
}

run();

```
<!-- No Retries [retries] -->

<!-- Start Error Handling [errors] -->
## Error Handling

[`MaesnError`](./src/models/errors/maesn-error.ts) is the base class for all HTTP error responses. It has the following properties:

| Property            | Type       | Description                                            |
| ------------------- | ---------- | ------------------------------------------------------ |
| `error.message`     | `string`   | Error message                                          |
| `error.statusCode`  | `number`   | HTTP response status code eg `404`                     |
| `error.headers`     | `Headers`  | HTTP response headers                                  |
| `error.body`        | `string`   | HTTP body. Can be empty string if no body is returned. |
| `error.rawResponse` | `Response` | Raw HTTP response                                      |

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
    const result = await maesn.accounting.getAccount({
      accountId: "<id>",
    });

    console.log(result);
  } catch (error) {
    if (error instanceof errors.MaesnError) {
      console.log(error.message);
      console.log(error.statusCode);
      console.log(error.body);
      console.log(error.headers);
    }
  }
}

run();

```

### Error Classes
**Primary error:**
* [`MaesnError`](./src/models/errors/maesn-error.ts): The base class for HTTP error responses.

<details><summary>Less common errors (6)</summary>

<br />

**Network errors:**
* [`ConnectionError`](./src/models/errors/http-client-errors.ts): HTTP client was unable to make a request to a server.
* [`RequestTimeoutError`](./src/models/errors/http-client-errors.ts): HTTP request timed out due to an AbortSignal signal.
* [`RequestAbortedError`](./src/models/errors/http-client-errors.ts): HTTP request was aborted by the client.
* [`InvalidRequestError`](./src/models/errors/http-client-errors.ts): Any input used to create a request is invalid.
* [`UnexpectedClientError`](./src/models/errors/http-client-errors.ts): Unrecognised or unexpected error.


**Inherit from [`MaesnError`](./src/models/errors/maesn-error.ts)**:
* [`ResponseValidationError`](./src/models/errors/response-validation-error.ts): Type mismatch between the data returned from the server and the structure expected by the SDK. See `error.rawValue` for the raw value and `error.pretty()` for a nicely formatted multi-line string.

</details>
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
