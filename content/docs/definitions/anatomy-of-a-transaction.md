---
title: The anatomy of a Transaction
description: This document identifies the lengthiest possible transaction and all the possible intermediate steps in the process.
author: Raveesh Agarwal
date: 22 Jan 2025
---
### Transaction
A transaction is the atom of finance. A transaction is an exchange of currency against value delivered.

### Customer
A customer is the party who initiates the transaction. Usually, they offer currency against value delivered.

### Vendor
The vendor is the other party of the transaction. The vendor delivers value and expects currency in exchange. It is usually on the vendor to deploy the sales software to enable the exchange

### RFQ
A request for quotation is the initiation of the sales process. When the customer is not sure of the value they want from the vendor, they initiate the process with a request for quotation. This usually has items that the customer is interested in.

### Quotation
A quotation is a reply from the vendor against the RFQ. This usually happens after rounds of clarification and offline conversation between the customer and the vendor. Once the vendor is confident about the customer wants, they release the quotation.
The vendor can also release multiple quotations to give the customer options.

### Order
An order is created when the customer knows exactly what they want from the vendor. The vendor can either accept the order, or reject it. 
Orders are a proof of what was asked from the vendor, not a proof of what the vendor has delivered.

### Estimate
Order is created when the customer has clarity on what they want. Accepting the order means the vendor understands what the customer wants. This does not necessarily mean that the vendor knows exactly what to charge.
When the vendor does not know the exact cost to customer for the value delivered, they use a tool called estimate. 
An estimate has to contain:
- Description of deliverable
- Expected ceiling amount
- (optional) Timeline of delivery
In case the customer accepts and signs the estimate, it means that the customer has agreed to pay up to the ceiling amount without further qualification. 
And the vendor has agreed that should the actual cost to customer exceed the ceiling amount, they would let the customer know and provide a new estimate.

### Invoice
Should the service be complete, or the items be packed, or subsequent orders be placed.
i.e. at the moment the vendor has complete confirmation of the value delivered, the vendor raises the invoice.
An invoice documents the `ask` for payment. It has parameters such as:
- Required Amount
- Payment Terms(Including Cash Discount)
- Details of the Payment Method
etc

### Customer Account
Known customers can have a customer account within the business that they can use to manage a consolidated payment structure beyond invoice. 
An invoice can be marked as paid through customer account and the finance team will then need to follow up with the customer on amount backlogs. (The invoice will be marked as paid).

### Receipt
For every payment the customer makes to the vendor, the customer should receive a receipt. The receipt can be against an invoice or against the customer account based upon the business lending scenario.
A receipt is a proof of payment made.

### Bill
In case of goods, the vendor needs to attach a bill against every shipment. A bill is the document for the goods present in a specific shipment.
In case one transaction will lead to multiple shipments, there will be one invoice, but separate bills attached to each shipment.
Usually bills are used to:
- manage inventory operations(for customer to credit to their inventory and vendors to debit)
- serve as a proof of date for warranty
In retail use cases, goods to be delivered are in the cart. So `billing` is the only step that the vendor needs to do.

### Return Transfer
Return transfer is the opposite of bill. This is used to insert items back into the inventory.
This should be used in conjunction with a credit note if the bill was invoiced.

### Credit Note
Credit note is appended to the invoice in case of returns. This is used for accounting for returns of invoiced items.
