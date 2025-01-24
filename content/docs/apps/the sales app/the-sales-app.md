---
draft: "true"
---

The sales app is the first implementation of a sales process. This app is used in corporate sales flows where it takes time and negotiation to get to a sales contract.

- the primary goal and scope of the sales app is till we get an order from the customer.
- as a secondary perspective we show order statuses once the orders are realised, but that is just so that the sales team(s) can hold the other teams accountable for delivery.

As such, the following lists are shown in the primary screen:
- RFQs
- Quotations
- Orders

Following the AARRR pirate metrics in marketing, marketing team converts leads into customers.
At the moment of the conversion, customer shows interest in some offering. This is a request for quotation.
## RFQs
RFQ, or request for quotation documents a lead’s interest in an offering. An RFQ object should ideally hold the answers to:
1. Where did the RFQ come from -> `origin`
2. Who is requesting the quotation -> `leadProfile`
3. What offering are they interested in -> `requestedOfferingDescription`
4. By when will they wait for the quotation(usually asked as `when do you plan to buy our offering`) -> `deadLine`
### `rfq.origin`
some surfaces through which an `rfq` can enter the sales system are:
- **email-outreach**- in this form of receiving, 
	- the `requestedOfferingDescription` is unclear.  An `inference AI agent` can be used for reading through the emails and:
		- push possible `rfq` in to the sales app
		- understand the requested offering and pick the offering the lead is interested in
	- the `leadProfile` is not as effective
		- we can use lead generation discovery services to supplement the lead profile with data available in the market.
	- `deadline` will most likely will require a manual follow-up
- **form-submission**- the sales app can offer embeddable forms to the funnel builder. 
	- business is in control of the `leadProfile`. They need to find the right balance between identifying the customer and their segment vs making the form accessible and simple. lead generation services can augment this as well.
	- drop downs and text fields can get early segmentation of lead‘s interest. Business decides how specific they want their `requestedOfferingDescription`
	- `deadline` can be an explicit or inferred option at form submission
- **ai-agent**- sales ai agents can be embedded in chatbots to get RFQs. they can combine the power of early segmentation that forms offers with the inference models to get to the best possible outcomes as possible. it will be up to us / agencies to train such agents at scale

### `rfq.leadProfile`
`leadProfile` is everything about the lead. Knowing more about the lead can help sales app users convert more into customers. This can be divided into:
1. Contact information
2. Segmentation
3. Conversion Factors
4. Past Interactions / Transactions
5. Warnings
A good sales app should be able to provide all the above information to the user on tap. This can use a mix of:
- lead generation services
- paid lists and 
- qualifying steps in the `ai agent / funnel form` design.

### `rfq.requestedOfferingDescription`
a lead enters the system, always with an initial interest. One lead can also have multiple interests, this can either be handled as multiple offerings in a single rfq or as separate rfqs.



This will help organisations to scale their sales functions effectively as each of their sales agents will have a good understanding of what the customer needs, and who the customer is.


## Quotations


## Orders



Operationally, the sales team takes over when the RFQ is received. The RFQ view is a view where the salesperson can see all the inbound interest. Their job here is to create a quotation for the request and respond. A customer accepting the RFQ should lead to creation of an order.

Quotations need to have the information on:
1. Who are we targeting
2. What are we selling
3. Date of Creation
4. Date till valid
Quotations can also be created independent of RFQs.
An interaction can enter the system starting at a quotation.

### Who are we Targeting
## CRM Integrations
### Opportunities
Sales app can have sales.rfq, sales.quotation and sales.order as three available columns for an opportunity kanban that auto populates and auto organises as the sales team continues their day to day on the sales app.
### Contact Details
Sales app can make available a list of rfqs, outbound offers ans orders for a specific contact so that a relationship manager can understand the history of outreach.